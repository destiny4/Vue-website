<template>
  <div>
    <div class="custom-area-area">
      <div>
        <p class='p-first'>工程案例</p>
        <p class='p-second'>Engineering case</p>

        <div class='custom-separator'>
          <q-separator color='primary' />
          <q-btn flat />
        </div>
      </div>
    </div>
    <article class='bg-case text-center'>
      <div class="bg-base-img column row-sm q-col-gutter-y-xl q-col-gutter-sm-x-xl items-start">
        <div class="col-4">
          <q-img src="statics/img/6@2x.png">
            <div class="absolute-bottom text-subtitle1 text-left">
              案例名称
            </div>
          </q-img>
        </div>

        <div class="col-4">
          <q-img src="statics/img/5@2x.png">
            <div class="absolute-bottom text-subtitle1 text-left">
              案例名称
            </div>
          </q-img>
        </div>

        <div class="col-4">
          <q-img src="statics/img/7@2x.png">
            <div class="absolute-bottom text-subtitle1 text-left">
              Caption
            </div>
          </q-img>
        </div>
      </div>
      <q-btn style='font-family: STHeitiSC-Light;font-size: 18px'
             flat
             label='全部案例 >'
             class='text-white'></q-btn>
    </article>
  </div>
</template>
<script>
export default {
  data () {
    return {
      imgArr: [{
        label: '案例名称', outClass: 'col-4', innerClass: 'absolute-bottom text-subtitle1 text-left', src: 'https://cdn.quasar.dev/img/parallax2.jpg'
      }, {
        label: '案例名称', outClass: 'col-4', innerClass: 'absolute-bottom text-subtitle1 text-left', src: 'https://cdn.quasar.dev/img/parallax2.jpg'
      }, {
        label: '案例名称', outClass: 'col-4', innerClass: 'absolute-bottom text-subtitle1 text-left', src: 'https://cdn.quasar.dev/img/parallax2.jpg'
      }]
    }
  }
}
</script>
<style lang="scss">
.bg-case {
  background-image: url("/statics/img/case-bg.png");
  padding: 3.5vw 12.5vw 0 12.5vw;
  .q-img {
    height: 28.8vw;
  }
}
.custom-area-area {
  padding: 0 12.5vw;
  margin: 80px 0 40px 0;
  .p-first {
    font-family: STHeitiSC-Medium;
    font-size: 36px;
    color: #000000;
    line-height: 36px;
    text-align: center;
  }
  .p-second {
    font-family: STHeitiSC-Medium;
    font-size: 18px;
    color: #91929e;
    line-height: 18px;
    text-align: center;
  }
}
@media (max-width: 600px) {
  .bg-base-img {
    .col-4 {
      width: 100%;
    }
  }
  .bg-case {
    .q-img {
      height: 80vw;
    }
  }
}
</style>
