<template>
<!-- about -->
<section class="about section" id="about">
  <div class="inner">
    <h2 class="title">ABOUT</h2>
    <div class="profile">
      <p class="profile-img">
        <img src="@/assets/about.jpg" alt="">
      </p>
      <div class="profile-body">
        <p>
          大学在学中から1年半のインターンを経て卒業後、新卒でWebサービス開発を担う会社に入社。コーダー/フロントエンドエンジニアとして開発を10年ほど経験。現在はフリーランスで業務委託案件をメインに受託中。<br>
        </p>
        <a href="https://github.com/Honoka-Y" target="_blank" rel="noopener"><img src="@/assets/ico_github.png" alt="github-icon">Github</a>
      </div>
    </div>
  </div>
</section>
<!-- /about -->
</template>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
/*--------------------------------
About
---------------------------------*/
.profile {
  display: flex;
  flex-wrap: wrap;
  max-width: 800px;
  margin: 0 auto;
}
.profile-img {
  width: 20%;
  margin-right: 30px;
  border-radius: 50%;
}
.profile-img img {
  border-radius: 50%;
}
.profile-body {
  flex: 1;
  text-align: left;
}
.profile-body a {
  color: #3a5b52;
}
.profile-body a:hover {
  opacity: .7 ;
}
.profile-body img {
  width: 30px;
  margin-right: 10px;
}
.profile-body p:not(:last-child) {
  margin-bottom: 30px;
}
/*media Queries 767
--------------------------------------*/
@media screen and (max-width: 767px) {
  /* About */
  .profile {
    display: block;
  }
  .profile-img {
    width: 150px;
    margin: 0 auto;
    margin-bottom: 25px;
  }
  .profile-body p:not(:last-child) {
    margin-bottom: 20px;
  }
  .profile-body a {
    display: block;
    width: 100px;
    margin: 0 auto;
  }
}
</style>
