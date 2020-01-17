<template>
  <q-page style="min-height:75vh">
    <q-carousel
      animated
      v-model="slide"
      arrows
      navigation
      infinite
      :autoplay="autoplay"
      navigation-icon='remove'
      class='custom-img'
    >
      <q-carousel-slide :name="1" img-src="https://s2.ax1x.com/2020/01/13/l7kejs.png" />
      <q-carousel-slide :name="2" img-src="https://s2.ax1x.com/2020/01/13/l7k9Bt.png" />
      <q-carousel-slide :name="3" img-src="https://cdn.quasar.dev/img/parallax1.jpg" />
    </q-carousel>
  </q-page>
</template>
<script>
export default {
  data () {
    return {
      slide: 1,
      autoplay: false
    }
  }
}
</script>
<style lang="scss">
    .q-carousel__navigation .q-btn {
        margin: 0
    }
  //  .q-carousel__navigation-inner .q-btn .q-icon, .q-btn .q-spinner{
  //       font-size: 2.715em
  //   }
    .custom-img{
      height:75vh
    }
</style>
