<template>
  <div class="container">
  <div class="header_link_box">
  <p class="link_home"><a href="">ホーム</a></p>
  <p class="link_profil"><a href="">生態(プロフィール)</a></p>
  </div>
    <div class="header__logo-box">
    <img src="@/assets/img/blog_title_img.png" alt="Logo" class="header__logo">
    <link rel="preconnect" href="https://fonts.gstatic.com">
<link href="https://fonts.googleapis.com/css2?family=Yusei+Magic&display=swap" rel="stylesheet">
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
</div>
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
}
.header_link_box{
display: flex;
justify-content: center;
font-family:'Yusei Magic', sans-serif;
}
.header_link_box .link_home{
padding:10px 30px;

}
.header_link_box .link_home a::after {
	content: '';
	position: absolute;
	top: 3%;
	left: 43%;
	width: 0;
	height: 0;
	background-color: rgba(185,155,0,0.5);
	border-radius: 50%;
	transition: 0.3s;
}

.header_link_box .link_home a:hover::after {
	width: 40px;
	height: 40px;
}
.header_link_box .link_profil{
padding:10px 30px;
}
.header_link_box .link_profil a::after {
	content: '';
	position: absolute;
	top: 3%;
	left: 50%;
	width: 0;
	height: 0;
	background-color: rgba(185,155,0,0.5);
	border-radius: 50%;
	transition: 0.3s;
}

.header_link_box .link_profil a:hover::after {
	width: 40px;
	height: 40px;
}

.img {
  width: 100%;
  height: 400px;
  object-fit: cover;
}
.title {
  display: block;
  font-family:'Yusei Magic', sans-serif;
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
