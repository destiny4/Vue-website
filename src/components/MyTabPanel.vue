<template>
  <div class="custom-product-area">
    <div>
      <p class='p-first'>优质产品</p>
      <p class='p-second'>Quality products</p>

      <div class='custom-separator'>
        <q-separator color='primary' />
        <q-btn flat />
      </div>

      <div class="custom-button column row-sm justify-between">
        <q-btn flat
               v-for="(item,index) in tabBtn"
               :key="index"
               @mouseover="btnTab(item.name)"
               :label="item.label" />
      </div>

      <q-tab-panels v-model="tab"
                    animated
                    transition-prev="scale"
                    transition-next="scale"
                    class="bg-white text-black text-center">
        <q-tab-panel name="mails">
          <div class='column row-sm product-detail'>
            <img src="https://www.xhjt1118.com/uploads/2018/07/231403218798.jpg"
                 title="装配式建筑"
                 alt="装配式建筑">
            <article class='detail column justify-start'>
              <p class='col-1'>装配式建筑</p>
              <p class='col'>所有建筑组件，包括墙体、楼板、楼梯、房顶，甚至护栏、装饰柱等，均采用自主研发生产的新型纤维建材预制生产；组件运输到施工现场，采用机械吊装、拼接粘合；可建设各类高低层建筑、别墅、定制化房型、水上建筑等...</p>
              <a class='col-1'
                 href="/article/type/87-1.html"
                 title="查看更多"
                 target="_blank">查看更多 >></a>
            </article>
          </div>
        </q-tab-panel>

        <q-tab-panel name="alarms">
          <div class='column row-sm product-detail'>
            <img src="https://www.xhjt1118.com/uploads/2018/07/231406195232.jpg"
                 title="新型墙体材料"
                 alt="新型墙体材料">
            <article class='detail column justify-start'>
              <p class='col-1'>新型墙体材料</p>
              <p class='col'>建筑建造中，隔墙板的工程是最关紧的局部之一，它的稳固性、安全性直接影响着整个工程的好坏，为了增强墙体的建造的安全性等，星河作为的轻质隔墙板厂家，用废弃木质纤维制造出抗强震、防虫、防潮、价格便宜的新型墙体材料...</p>
              <a class='col-1'
                 href="/article/type/87-1.html"
                 title="查看更多"
                 target="_blank">查看更多 >></a>
            </article>
          </div>
        </q-tab-panel>

        <q-tab-panel name="movies">
          <div class='column row-sm product-detail'>
            <img src="https://www.xhjt1118.com/uploads/2018/07/231406448004.jpg"
                 title="装饰装修建材"
                 alt="装饰装修建材">
            <article class='detail column justify-start'>
              <p class='col-1'>装饰装修建材</p>
              <p class='col'>在21世纪的中国，随着市场的进一步开放，出现了越来越多样式新颖的家具。在基本的生活需求得到满足后，一些人开始注重家居生活的质量，特别是家居产品对于健康的影响，因此环保家具渐渐被人们所重视，绿色消费风潮也推动了环保家具的发展...</p>
              <a class='col-1'
                 href="/article/type/87-1.html"
                 title="查看更多"
                 target="_blank">查看更多 >></a>
            </article>
          </div>
        </q-tab-panel>

        <q-tab-panel name="four">
          <div class='column row-sm product-detail'>
            <img src="https://www.xhjt1118.com/uploads/2018/07/231356282820.jpg"
                 title="市政工程部品"
                 alt="市政工程部品">
            <article class='detail column'>
              <p class='col-1'>市政工程部品</p>
              <p class="col">城市正在以史无前例的速度和规模发生扩张，纤维建材打造全新的市政工程部品...</p>
              <a class="col-1"
                 href="/article/type/87-1.html"
                 title="查看更多"
                 target="_blank">查看更多 >></a>
            </article>
          </div>
        </q-tab-panel>

        <q-tab-panel name="five">
          <div class='column row-sm product-detail'>
            <img src="https://www.xhjt1118.com/uploads/2018/07/231407069036.jpg"
                 title="植物纤维桥"
                 alt="植物纤维桥">
            <article class='detail column justify-start'>
              <p class='col-1'>植物纤维桥</p>
              <p class='col'>2016年4月23日，星河新型建材在四川绵阳市三台县建造的植物纤维桥，历时45分钟。该桥跨度17.5米，宽7.6米，自重56.5吨，承重100吨，承重可达500吨，建造采用的材料为星河自主研发的SGC新型建材，不用钢筋水泥。该桥已于2016年8月17日正式通车...</p>
              <a class='col-1'
                 href="/article/type/87-1.html"
                 title="查看更多"
                 target="_blank">查看更多 >></a>
            </article>
          </div>
        </q-tab-panel>

        <q-tab-panel name="six">
          <div class='column row-sm product-detail'>
            <img src="https://www.xhjt1118.com/uploads/2018/07/231404318113.jpg"
                 title="集成房屋建筑"
                 alt="集成房屋建筑">
            <article class='detail column justify-start'>
              <p class='col-1'>集成房屋建筑</p>
              <p class='col'>建筑结构模块均采用星河建材预制生产，可拆卸、可移动、不破坏土地，节能、节地、节材、节水、环保；采用笼式结构，专利技术粘合固定，具有良好的抗震性能...</p>
              <a class='col-1'
                 href="/article/type/87-1.html"
                 title="查看更多"
                 target="_blank">查看更多 >></a>
            </article>
          </div>
        </q-tab-panel>
      </q-tab-panels>
    </div>
  </div>
</template>
<script>
export default {
  data () {
    return {
      tab: 'mails',
      tabBtn: [{
        label: '装配式建筑', name: 'mails'
      }, {
        label: '新型墙体材料', name: 'alarms'
      }, {
        label: '装饰装修建材', name: 'movies'
      }, {
        label: '市政工程部品', name: 'four'
      }, {
        label: '植物纤维桥', name: 'five'
      }, {
        label: '集成房屋建筑', name: 'six'
      }]
    }
  },
  methods: {
    btnTab: function (name) {
      this.tab = name
    }
  }
}
</script>
<style lang="scss">
.custom-separator {
  margin-bottom: 45px;
  margin-top: 25px;
  position: relative;
  .q-btn {
    position: absolute;
    left: 0;
    right: 0;
    margin: 0 auto;
    width: 80px;
    height: 20px;
    top: -10px;
    background: #03aae5;
  }
}
.custom-product-area {
  padding: 0 12.5vw;
  margin: 80px 0;
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
  .q-tab-panels {
    margin-top: 67px;
  }
  .q-tab-panel {
    padding: 0;
    .product-detail {
      flex-wrap: nowrap;
      .detail {
        margin-left: 10px;
      }
      .detail p:nth-child(1) {
        font-size: 24px;
        color: #f7a30c;
        margin: 30px 0px;
        text-align: left;
      }
      .detail p:nth-child(2) {
        text-align: justify;
        font-size: 18px;
        color: #535353;
        letter-spacing: 4px;
        line-height: 31px;
      }
      a {
        background: #595959;
        display: block;
        height: 40px;
        width: 124px;
        text-align: center;
        line-height: 40px;
        color: white;
        border-radius: 10px;
        text-decoration: none;
      }
    }
    img {
      height: 31.25vw;
    }
  }
}
.custom-button {
  .q-btn {
    font-family: STHeitiSC-Medium;
    font-size: 18px;
    color: #ffffff;
    background: #03aae5;
  }
  .q-btn:hover {
    background: #086585;
  }
}
@media (max-width: 600px) {
  .custom-button {
    align-items: center;
    button {
      width: 100%;
    }
  }
  .custom-product-area {
    .q-tab-panel {
      .product-detail {
        .detail p:nth-child(1) {
          margin: 10px 0;
        }
      }
      img {
        height: 50vw;
      }
    }
  }
  .custom-button :not(:last-child) {
    margin-bottom: 10px;
  }
}
</style>
