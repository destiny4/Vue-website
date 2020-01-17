<template>
  <q-layout view="hHh LpR fff">
    <q-header v-model="head"
              reveal
              elevated
              class="bg-white text-black shadow-2">
      <my-tool-bar></my-tool-bar>
    </q-header>

    <q-page-container>
      <image-side></image-side>
      <my-tab-panel></my-tab-panel>
      <my-case></my-case>
      <my-news></my-news>
    </q-page-container>

    <q-footer>
      <my-footer></my-footer>
    </q-footer>

  </q-layout>
</template>

<script>
import ImageSide from 'components/ImageSlide'
import MyToolBar from 'components/MyToolBar'
import MyTabPanel from 'components/MyTabPanel'
import MyCase from 'components/MyCase'
import MyNews from 'components/MyNews'
import MyFooter from 'components/MyFooter'
export default {
  components: {
    ImageSide, MyToolBar, MyTabPanel, MyCase, MyNews, MyFooter
  },
  data () {
    return {
      head: true
    }
  }
}
</script>
<style scoped lang="scss">
</style>
