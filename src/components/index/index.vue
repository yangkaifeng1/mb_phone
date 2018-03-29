<template>
	<div class="slider-wrapper" v-if="recommands.length>0">
		<slider>
			<div v-for="item in recommands">
				<a >
					<img class="needsclick" :src="item">
				</a>
			</div>
		</slider>
	</div>
</template>

<script>
import Slider from 'base/slider/slider'

export default{	
	data() {
		return{
			recommands: [
					'https://www.zjmb158.com/public/attachment/201801/25/13/5a6968b212e26.jpg',
					'https://www.zjmb158.com/public/attachment/201803/16/09/5aab20b5d2c1b.jpg',
					'https://www.zjmb158.com/public/attachment/201801/18/16/5a6055e58c444.png',
					'https://www.zjmb158.com/public/attachment/201801/18/10/5a6004b381463.png',
					'https://www.zjmb158.com/public/attachment/201801/18/10/5a6002fcb3943.jpg'
				]
		}
	},
	components: {
		Slider
	}
}
</script>

<style lang="less" scoped>
	.slider-wrapper{
				position: relative;
				width: 100%;
				overflow: hidden;
			}
</style>