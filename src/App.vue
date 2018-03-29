<template>
  <div id="app">
    <mb-header></mb-header>
    <router-view/>
  </div>
</template>

<script>
import MbHeader from './components/mb-header/mb-header'

export default {
  components: {
    MbHeader
  }
}
</script>

<style>
</style>
