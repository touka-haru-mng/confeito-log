<template>
  <div class="container">
    <div>
      <NuxtLogo />
      <h1 class="title">
        こんぺいとう育成日記
      </h1>
      <div class="links">
        <van-button icon="smile-comment" round type="primary" size="normal" color="#7232dd">profile</van-button>
        <van-button icon="gem" round type="primary" size="normal" color="#7232dd" plain>オタ活</van-button>
        <van-button icon="fire-o" round type="primary" size="normal" color="linear-gradient(to right, #ff6034, #ee0a24)">
          注意事項
        </van-button>
      </div>
    </div>
  </div>
</template>

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
</style>
