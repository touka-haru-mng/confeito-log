<template>
<div class="container">
<div>
<h1 class="title">
こんぺいとうの生体
</h1>

<div class="section">

<div class="flex">
<img src="@/assets/img/Img.png" alt="Logo" class="profile_img">
<p class="profile_text">
こんぺいとうの生体記録です。
<br>オタクで引きこもりで飽き性なこんぺいとう…。
<br>日々のたわいないことをぼちぼち語っていきます。
<br>更新も日によってしたりしなかったりですが
<br>生暖かい目で見守ってください。
</p>
</div>

</div>
</div>
</div>
</template>
<style>
.container {
align-items: center;
justify-content: center;
display: flex;
}

.title {
  font-family:"Yu Gothic", "游ゴシック", YuGothic, "游ゴシック体";
  margin: 10px 50px 20px;
  font-weight: 300;
  padding: 1em;
  border: 3px solid #ccc;
  border-radius: 3em .7em 2em .7em/.7em 2em .7em 3em;
  text-align: center;
}



.flex{
  display: flex;
  align-items: center;
}
.flex .profile_img  {
vertical-align: middle;
}

.flex .profile_text {
background: #f8f0d7;
  border-left: 5px dotted rgba(0,0,0,.1);
  box-shadow: 0 0 0 5 #f8f0d7;
  padding: 6em 1em 6em;
  margin: 1em 5px;
}

.flex .profile_text p {
margin: 0;
  padding: 0;
}

</style>
