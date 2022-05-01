<template>
  <div class="container">
    <div>
    <div class="header__logo-box">
    <img src="@/assets/img/Img.png" alt="Logo" class="header__logo">

  </div>
      <h1 class="title">
        こんぺいとう育成日記
      </h1>
      <div class="card-group">
    <div class="card">
      <div class="card__imgframe"></div>
      <div class="card__textbox">
        <div class="card__titletext">
          タイトルがはいります。タイトルがはいります。
        </div>
        <div class="card__overviewtext">
          概要がはいります。概要がはいります。概要がはいります。概要がはいります。
        </div>
        <div class="card-link">
          <a href="#">HOME</a>
          <a href="#">FAQ</a>
          <a href="#">PRIVACY</a>
        </div>
      </div>
    </div>
    <div class="card">
      <div class="card__imgframe"></div>
      <div class="card__textbox">
        <div class="card__titletext">
          タイトルがはいります。タイトルがはいります。
        </div>
        <div class="card__overviewtext">
          概要がはいります。概要がはいります。概要がはいります。概要がはいります。
        </div>
        <div class="card-link">
          <a href="#">HOME</a>
          <a href="#">FAQ</a>
          <a href="#">PRIVACY</a>
        </div>
      </div>
    </div>
    <div class="card">
      <div class="card__imgframe"></div>
      <div class="card__textbox">
        <div class="card__titletext">
          タイトルがはいります。タイトルがはいります。
        </div>
        <div class="card__overviewtext">
          概要がはいります。概要がはいります。概要がはいります。概要がはいります。
        </div>
        <div class="card-link">
          <a href="#">HOME</a>
          <a href="#">FAQ</a>
          <a href="#">PRIVACY</a>
        </div>
      </div>
    </div>
    <div class="card">
      <div class="card__imgframe"></div>
      <div class="card__textbox">
        <div class="card__titletext">
          タイトルがはいります。タイトルがはいります。
        </div>
        <div class="card__overviewtext">
          概要がはいります。概要がはいります。概要がはいります。概要がはいります。
        </div>
        <div class="card-link">
          <a href="#">HOME</a>
          <a href="#">FAQ</a>
          <a href="#">PRIVACY</a>
        </div>
      </div>
    </div>
  </div>

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
.card-group{
  margin-left: auto;
  margin-right: auto;

  max-width: 640px;
  width: 90%;
  height: auto;

   /* 注目 */
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  flex-wrap: wrap;
}

/* 注目 */
.card-group > :nth-child(2n){
  margin-left: 20px;
}
/* 注目 */
.card-group > :nth-child(n+3){
  margin-top: 20px;
}

.card:hover {
  transform: translateY(-5px);
  box-shadow: 0 7px 34px rgba(50,50,93,.1), 0 3px 6px rgba(0,0,0,.08);
  transition: all .5s;
}

.card{

  /* 注目 */
  width: calc((100% - 20px * 1) / 2);

  height: auto;
  border-radius: 8px;
  overflow: hidden;
  box-shadow: 0 4px 15px rgba(0,0,0,.2)
}

.card__imgframe{
  width: 100%;
  height: auto;
  padding-top: 56.25%;
  background: #bbb;
  box-sizing: border-box;
}

.card__textbox{
  width: 100%;
  height: auto;
  padding: 20px 18px;
  background: #fff;
  box-sizing: border-box;
}

.card__textbox > * + *{
  margin-top: 10px;
}

.card__titletext{
  font-size: 20px;
  font-weight: bold;
  line-height: 125%;
}

.card__overviewtext{
  font-size: 12px;
  line-height: 150%;
}
.card-link {
  text-align: center;
  border-top: 1px solid #eee;
  padding: 20px;
}
.card-link a {
  text-decoration: none;
  color: #4f96f6;
  margin: 0 10px;
}
.card-link a:hover {
  color: #6bb6ff;
}
</style>
