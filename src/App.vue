<template>
  <div id="app">
    <Main></Main>
  </div>
</template>

<script>
import Vue from 'vue'
import VueCoreVideoPlayer from 'vue-core-video-player'
import Main from './components/Main.vue'

Vue.use(VueCoreVideoPlayer, {
  lang: 'zh-CN'
})

export default {
  name: 'App',
  components: {
    Main
  }
}
</script>

<style>

</style>
