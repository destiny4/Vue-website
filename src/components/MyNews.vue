<template>
  <div class="custom-area-area">
    <div>
      <p class='p-first'>新闻动态</p>
      <p class='p-second'>News information</p>

      <div class='custom-separator'>
        <q-separator color='primary' />
        <q-btn flat />
      </div>
    </div>

    <div class="bg-news-img column row-sm justify-between">
      <div class="news-area margin-bottom row no-wrap">
        <q-img src="statics/img/8@2x.png"
               alt="餐具">
        </q-img>
        <div class='news-content'>
          <p>新闻标题</p>
          <div>
            {{newsContent}}
            <span>[详情]</span>
          </div>
        </div>
      </div>

      <div class="news-area margin-bottom row no-wrap">
        <q-img src="statics/img/8@2x.png"
               alt="餐具">
        </q-img>
        <div class='news-content'>
          <p>新闻标题</p>
          <div>
            {{newsContent}}
            <span>[详情]</span>
          </div>
        </div>
      </div>

      <div class="news-area row no-wrap">
        <q-img src="statics/img/8@2x.png"
               alt="餐具">
        </q-img>
        <div class='news-content'>
          <p>新闻标题</p>
          <div>
            {{newsContent}}
            <span>[详情]</span>
          </div>
        </div>
      </div>

      <div class="news-area row no-wrap">
        <q-img src="statics/img/8@2x.png"
               alt="餐具">
        </q-img>
        <div class='news-content'>
          <p>新闻标题</p>
          <div>
            {{newsContent}}
            <span>[详情]</span>
          </div>
        </div>
      </div>
    </div>

    <q-btn style='display: block;margin: 0 auto;color:#1890FF;font-family: STHeitiSC-Light;font-size: 18px'
           flat
           label='全部新闻 >'></q-btn>
  </div>
</template>
<script>
export default {
  data () {
    return {
      newsContent: '信息文本信息文本信息文本信息文本信息文本信息文本信息文本信息文本信息文本信息文本信息文本'
    }
  }
}
</script>
<style lang="scss">
.bg-news-img {
  // .margin-bottom {
  //   margin-bottom: 15px;
  // }
  .news-area {
    margin-bottom: 30px;
    width: 48%;
    .q-img {
      width: 67%;
    }
    .news-content {
      width: 16.67vw;
      margin-left: 1.3vw;
      p {
        font-family: STHeitiSC-Medium;
        font-size: 24px;
      }
      div {
        font-family: STHeitiSC-Light;
        font-size: 16px;
        color: #333333;
        text-align: justify;
      }
      span {
        color: #1890ff;
      }
    }
  }
}
@media (max-width: 600px){
  .bg-news-img {
       .news-area{
             display: flex;
    flex-direction: column;
    align-items: center;
         width: 100%;
         .news-content{
           width: 100%;
           p{
             text-align: center
           }
         }
       }
    }
}
</style>
