<template>
  <div class="footer-area column row-sm justify-between">
    <div class='left-footer'>
      <div class='left-top'>
        <p>联系我们</p>
        <span>Contact us</span>
      </div>
      <p>
        <q-icon name='phone'></q-icon> <span>400-666-6666</span>
        <q-icon style='margin-left:30px'
                name='email'></q-icon> <span>673546699@qq.com</span>
      </p>
      <p>
        <q-icon name='phone_iphone'></q-icon> <span>189-0987-5658</span>
        <span style='margin-left:30px'>130-8876-0324</span>
      </p>
      <p>
        <q-icon name='my_location'></q-icon> <span>北京市朝阳区天安门广场32号</span>
      </p>
    </div>
    <div class='right-footer row justify-center'>
      <q-img src="statics/img/8@2x.png"
             alt="餐具">
      </q-img>
    </div>
  </div>
</template>
<script>
export default {
  data () {
    return {
      newsContent: ''
    }
  }
}
</script>
<style lang="scss">
.footer-area {
  padding: 0 12.5vw;
  background-color: #494949;
  font-family: STHeitiSC-Light;
  color: #ffffff;
  letter-spacing: 0.2px;
  span {
    margin-left: 15px;
  }
  .left-footer {
    width: 48%;
    font-size: 16px;
    .left-top {
      margin-bottom: 30px;
      p {
        margin: 15px 0 0 0;
        font-size: 36px;
        letter-spacing: 0.45px;
      }
      span {
        font-size: 18px;
        margin: 0;
      }
    }
  }
  .right-footer {
    width: 48%;
    .q-img {
      width: 50%;
    }
  }
}

@media (max-width: 600px) {
  .footer-area {
    .left-footer {
      width: 100%;
      font-size: 13px;
      .left-top {
        margin-bottom: 30px;
        p {
          margin: 8px 0 0 0;
          font-size: 30px;
          letter-spacing: 0.45px;
        }
        span {
          font-size: 15px;
          margin: 0;
        }
      }
    }
    .right-footer {
      width: 100%;
      .q-img {
        width: 100%;
      }
    }
  }
}
</style>
