<template>
  <!-- 大枠（今は中心に集まるようにしている -->
  <!-- background-image:url("\assets\img\background.jpg");は悩む -->
  <body class="container">

  <!-- フォントデザインの読み込み -->
  <link rel="preconnect" href="https://fonts.gstatic.com">
  <link href="https://fonts.googleapis.com/css2?family=Yusei+Magic&display=swap" rel="stylesheet">

  <!-- ホーム画面上部のリンクボタン -->
  <ul class="header_link_box">
  <li class="link_home"><a href="">ホーム</a></li>
  <li class="link_profil"><a href="">生態(プロフィール)</a></li>
  </ul>

    <div class="header__logo-box">
    <img src="@/assets/img/blog_title_img.png" alt="Logo" class="header__logo">
    <h1 class="title">
      こんぺいとうにっき
    </h1>
    </div>
      <div class="links">
        <van-button @click="profilebutton" icon="smile-comment" round type="primary" size="large" color="#3299dd">日々のぼやき</van-button>
        <van-button icon="gem" round type="primary" size="normal" color="#3299dd" plain>オタかつ</van-button>
        <van-button icon="fire-o" round type="primary" size="normal" color="#ddda32">
          注意
        </van-button>
      </div>
</body>
</template>
<script>
export default {
  methods: {
    profilebutton() {
      this.$router.push('/profile')
    },
  },
}
</script>

<style>

.container {
  margin: 0 auto;
  min-height: 100vh;
  justify-content: center;
  align-items: center;
  text-align: center;
  font-family:'Yusei Magic', sans-serif;
  background-color: #fdf5e6;
}

.header_link_box {
  display: flex;
  text-align: center;
  justify-content: center;
  padding: 20px;
}

.header_link_box li {
margin-left: 20px;
}

.img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
.title {
  display: block;
  font-weight: 300;
  font-size: 30px;
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
  font-family:'Yusei Magic', sans-serif;
}
.van-button{
    width: 150px;
    height: 120px;
    font-size:20px;
}
</style>
