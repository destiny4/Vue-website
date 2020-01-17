<template>
  <q-toolbar class="column row-sm">
    <img style='height:78px;'
         src="statics/img/logo@2x.png" />

    <q-space />
    <q-btn-group flat
                 class="column row-sm custom-header">
      <q-btn-dropdown color="transparent"
                      text-color="block"
                      dropdown-icon="keyboard_arrow_down"
                      label="企业介绍">
        <q-list class='custom-list'>
          <q-item clickable
                  v-close-popup
                  @click="onItemClick">
            <q-item-section>
              <q-item-label>企业简介</q-item-label>
            </q-item-section>
          </q-item>

          <q-item clickable
                  v-close-popup
                  @click="onItemClick">
            <q-item-section>
              <q-item-label>企业文化与策略</q-item-label>
            </q-item-section>
          </q-item>

          <q-item clickable
                  v-close-popup
                  @click="onItemClick">
            <q-item-section>
              <q-item-label>人才团队</q-item-label>
            </q-item-section>
          </q-item>

          <q-item clickable
                  v-close-popup
                  @click="onItemClick">
            <q-item-section>
              <q-item-label>企业架构</q-item-label>
            </q-item-section>
          </q-item>
        </q-list>
      </q-btn-dropdown>

      <q-btn-dropdown color="transparent"
                      text-color="block"
                      dropdown-icon="keyboard_arrow_down"
                      label="新闻动态">
        <q-list class='custom-list'>
          <q-item clickable
                  v-close-popup
                  @click="onItemClick">
            <q-item-section>
              <q-item-label>国家政策</q-item-label>
            </q-item-section>
          </q-item>
          <q-item clickable
                  v-close-popup
                  @click="onItemClick">
            <q-item-section>
              <q-item-label>行业资讯</q-item-label>
            </q-item-section>
          </q-item>
        </q-list>
      </q-btn-dropdown>

      <q-btn-dropdown color="transparent"
                      text-color="block"
                      dropdown-icon="keyboard_arrow_down"
                      label="在线视听">
        <q-list class='custom-list'>
          <q-item clickable
                  v-close-popup
                  @click="onItemClick">
            <q-item-section>
              <q-item-label>影视播报</q-item-label>
            </q-item-section>
          </q-item>
          <q-item clickable
                  v-close-popup
                  @click="onItemClick">
            <q-item-section>
              <q-item-label>企业信息发布</q-item-label>
            </q-item-section>
          </q-item>
        </q-list>
      </q-btn-dropdown>

      <q-btn-dropdown color="transparent"
                      text-color="block"
                      dropdown-icon="keyboard_arrow_down"
                      label="技术介绍">
        <q-list class='custom-list'>
          <q-item clickable
                  v-close-popup
                  @click="onItemClick">
            <q-item-section>
              <q-item-label>技术原理</q-item-label>
            </q-item-section>
          </q-item>
          <q-item clickable
                  v-close-popup
                  @click="onItemClick">
            <q-item-section>
              <q-item-label>技术成果</q-item-label>
            </q-item-section>
          </q-item>
          <q-item clickable
                  v-close-popup
                  @click="onItemClick">
            <q-item-section>
              <q-item-label>生产工艺</q-item-label>
            </q-item-section>
          </q-item>
          <q-item clickable
                  v-close-popup
                  @click="onItemClick">
            <q-item-section>
              <q-item-label>安装流程</q-item-label>
            </q-item-section>
          </q-item>
        </q-list>
      </q-btn-dropdown>

      <q-btn-dropdown color="transparent"
                      text-color="block"
                      dropdown-icon="keyboard_arrow_down"
                      label="工程案例">
        <q-list class='custom-list'>
          <q-item clickable
                  v-close-popup
                  @click="onItemClick">
            <q-item-section>
              <q-item-label>工程案例展示</q-item-label>
            </q-item-section>
          </q-item>
        </q-list>
      </q-btn-dropdown>

      <q-btn-dropdown color="transparent"
                      text-color="block"
                      dropdown-icon="keyboard_arrow_down"
                      label="服务系统">
        <q-list class='custom-list'>
          <q-item clickable
                  v-close-popup
                  @click="onItemClick">
            <q-item-section>
              <q-item-label>技术合作</q-item-label>
            </q-item-section>
          </q-item>
          <q-item clickable
                  v-close-popup
                  @click="onItemClick">
            <q-item-section>
              <q-item-label>
                项目招商
              </q-item-label>
            </q-item-section>
          </q-item>
          <q-item clickable
                  v-close-popup
                  @click="onItemClick">
            <q-item-section>
              <q-item-label>工程承揽</q-item-label>
            </q-item-section>
          </q-item>
          <q-item clickable
                  v-close-popup
                  @click="onItemClick">
            <q-item-section>
              <q-item-label>建房拎包入住一站式服务</q-item-label>
            </q-item-section>
          </q-item>
        </q-list>
      </q-btn-dropdown>

      <q-btn-dropdown color="transparent"
                      text-color="block"
                      dropdown-icon="keyboard_arrow_down"
                      label="联系我们">
        <q-list class='custom-list'>
          <q-item clickable
                  v-close-popup
                  @click="onItemClick">
            <q-item-section>
              <q-item-label>在线咨询</q-item-label>
            </q-item-section>
          </q-item>
          <q-item clickable
                  v-close-popup
                  @click="onItemClick">
            <q-item-section>
              <q-item-label>留言/投诉</q-item-label>
            </q-item-section>
          </q-item>
        </q-list>
      </q-btn-dropdown>
    </q-btn-group>
  </q-toolbar>
</template>

<script>
export default {
  methods: {
    onItemClick () {
      console.dir(arguments)
    }
  }
}
</script>

<style scoped lang="scss">
@media (min-width: 600px) {
  .custom-header {
    height: 86px;
    button {
      font-family: STHeitiSC-Medium;
      font-size: 18px;
      color: #000000;
    }
  }
}
@media (max-width: 600px) {
  .custom-header {
    align-items: center;
  }
}
.custom-list {
  .justify-center,
  .flex-center {
    align-items: center;
  }
  .q-item__label {
    font-family: STHeitiSC-Medium;
    font-size: 16px;
    color: #000000;
  }
}
</style>
