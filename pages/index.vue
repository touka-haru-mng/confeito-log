<template>
  <div class="container">
    <div>
    <div class="header__logo-box">
    <img src="@/assets/img/Img.png" alt="Logo" class="header__logo">

  </div>
      <h1 class="title">
        こんぺいとう育成日記
      </h1>
      <div class="links">
        <van-button @click="profilebutton" icon="smile-comment" round type="primary" size="large" color="#3299dd">せいたい</van-button>
        <van-button icon="gem" round type="primary" size="normal" color="#3299dd" plain>オタかつ</van-button>
        <van-button icon="fire-o" round type="primary" size="normal" color="#ddda32">
          ちゅうい
        </van-button>
        </div>

      </div>
  </div>
    </div>
</template>
<script>
export default {
  methods: {
    profilebutton: function() {
 　　　// do something

      this.$router.push('/profile')
    },
  },
}
</script>
<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  display: block;
  font-family:"Yu Gothic", "游ゴシック", YuGothic, "游ゴシック体";
  font-weight: 300;
  font-size: 50px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
.van-button{
    width: 150px;
    height: 120px;
    font-size:20px;
}
</style>
