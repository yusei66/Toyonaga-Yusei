<template>
  <div class="container">
    <div class="firstView">
      <div class="firstView_contents1">
        とよなが
      </div>
      <div class="firstView_contents2">
        ＃ぼんやり、ゆらゆら
      </div>
      <div class="firstView_contents3">
        #豊永の肩には象がいる
      </div>
      <div class="firstView_contents4">
        follow me
      </div>
      <div class="firstView_contents5">
        <nav tabindex="-1" class="menu">
          <ul tabindex="-1" class="menu-ul">
            <li><a href="#">リンク</a></li>
            <li><a href="#">リンク</a></li>
            <li><a href="#">リンク</a></li>
            <li><a href="#">リンク</a></li>
            <li><a href="#">リンク</a></li>
          </ul>
        </nav>
      </div>
    </div>
    <div class="about">
      <div class="aboutImg">
        <div class="aboutImg1 image">
          ::before
        </div>
        <style>
          .about:before {
            background-image: url("../static/sample.jpg")
          }
        </style>
      </div>
      <div class="aboutContents">
        <h2 class="text sd">about</h2>
        <h3 class="text sd h3-1">”ゆれる”を創る</h3>
        <h3 class="text sd h3-2">それをココから。</h3>
        <p class="text sd">
          "何か、なだらかなアシタに昨日の香りを感じる、今日このごろ。"
          <br>
          "今日より、明日がよくなるとお思いですか？"
          <br>
          "意外と変わりませんよ。明日も今日も。"
        </p>
        <div class="readMore">
        </div>
      </div>

      <div class="image sd">
        ::before
        <div class="imgMask">
          <p>ever yesterday never today...</p>
        </div>
        <style>.sd:before {
          background-image: url("../static/sample.jpg")
        }</style>
      </div>
      <div class="image sd">
        ::before
        <style>.sd:before {
          background-image: url("../static/sample.jpg")
        }</style>
      </div>
      <div class="aboutBackground"></div>
    </div>

    <div class="works">
      <div class="worksContents">
        <h1 class="worksTitle">Works</h1>
        <div class="worksCard">
          <div class="card card-skin">
            <div class="card__imgframe"></div>
            <div class="card__textbox">
              <div class="card__titletext">
                タイトルがはいります。タイトルがはいります。
              </div>
              <div class="card__overviewtext">
                概要がはいります。概要がはいります。概要がはいります。概要がはいります。
              </div>
            </div>
          </div>
          <div class="card card-skin">
            <div class="card__imgframe"></div>
            <div class="card__textbox">
              <div class="card__titletext">
                タイトルがはいります。タイトルがはいります。
              </div>
              <div class="card__overviewtext">
                概要がはいります。概要がはいります。概要がはいります。概要がはいります。
              </div>
            </div>
          </div>
          <div class="card card-skin">
            <div class="card__imgframe"></div>
            <div class="card__textbox">
              <div class="card__titletext">
                タイトルがはいります。タイトルがはいります。
              </div>
              <div class="card__overviewtext">
                概要がはいります。概要がはいります。概要がはいります。概要がはいります。
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="project">
      <div class="projectTitle">
        <div class="projectText1">
          <h2>pro</h2>
        </div>
        <div class="projectTexts">
          <img src="../static/sample01.jpg" height="235px" width="350px"/>
          <div class="projectText2"><h2>ject</h2></div>
        </div>
      </div>
      <div class="projectContents1">
        <img src="../static/sample02.jpg" height="235px" width="350px"/>
        <div class=" projectTextbox1">今日はすごく良い天気になりました。</div>
      </div>
      <div class="projectContents2">
        <img src="../static/sample02.jpg" height="235px" width="350px"/>
        <div class=" projectTextbox2">今日はすごく良い天気になりました。</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style>
.firstView {
  width: 100%;
  height: 100vh;
  padding: 40px 30px;
  position: relative;
}

.firstView_contents2 {
  position: absolute;
  left: 30px;
  bottom: 40px;
  -ms-writing-mode: tb-rl;
  writing-mode: vertical-rl;
}

.firstView_contents3 {
  position: absolute;
  right: 30px;
  bottom: 40px;
}

.firstView_contents4 {
  transform: rotate(90deg);
  position: absolute;
  right: 0;
  bottom: 50%;
}

.menu {
  position: fixed;
  top: 0;
  right: 0;
  outline: none;
  z-index: 100;
}

.menu::before {
  position: absolute;
  top: 50px;
  right: 40px;
  cursor: pointer;
  /*
     アイコンは、はてなブログのデフォルトアイコン使用しています。
 */
  font-family: blogicon;
  content: "\f003";
  font-size: 30px;
  line-height: 1;
}

.menu-ul {
  position: absolute;
  top: 0;
  right: -80vw;
  margin: 0;
  list-style: none;
  width: 80vw;
  height: 100vh;
  background: #fff;
  padding: 20px;
  box-sizing: border-box;
  outline: none;
  transition: right 0.4s 0.1s;
}

.menu-ul::after {
  position: absolute;
  content: "";
  top: 0;
  right: 0;
  width: 0;
  height: 0;
  z-index: -1;
  background: rgb(0, 0, 0);
  opacity: 0;
  transition: opacity 0.4s 0.1s,
  width 0s 0.5s,
  height 0s 0.5s;
}

.menu:focus .menu-ul {
  right: 0;
  transition: right 0.5s;
}

.menu-ul:focus {
  right: -80vw;
}

.menu:focus .menu-ul::after {
  width: 180vw;
  height: 100vh;
  opacity: 0.4;
  transition: opacity 0.5s;
}

.about {
  align-content: center;
  align-items: center;
  background: #FFFFFF;
  flex: none;
  flex-direction: column;
  flex-wrap: nowrap;
  height: auto;
  justify-content: flex-start;
  margin: 0 0 0 0;
  padding: 0 0 0 0;
  transform: translate(0px, 0px);
  width: 100%;
  z-index: 0;
  max-width: 100%;
}

.aboutContents {
  align-content: flex-start;
  align-items: flex-start;
  background: rgba(0, 0, 0, 0.0);
  flex: none;
  flex-direction: column;
  flex-wrap: nowrap;
  height: auto;
  justify-content: flex-start;
  margin: 140px 60px 0 60px;
  width: 650px;
  max-width: calc(100% - 120px);
}

.aboutImg {
  align-content: flex-start;
  align-items: flex-start;
  flex-direction: row;
  flex-wrap: nowrap;
  justify-content: flex-start;
  margin: -100px 0 0 0;
  padding: 0;
  width: 100%;
  max-width: 100%;
}

.aboutImg1 {
  margin: 0 0 0 0;
  width: 90%;
  max-width: 90%;
  height: 80vh;
}

.aboutContents h2 {
  color: #FFFFFF;
  flex: none;
  font-family: Helvetica;
  font-size: 64px;
  font-weight: 600;
  height: auto;
  letter-spacing: 0.1em;
  line-height: 1;
  margin: 0 0 0 0;
  text-align: left;
  width: 100%;
  max-width: 100%;
  justify-content: flex-start;
}

.h3-1{
  color: #FFFFFF;
  flex: none;
  font-family: '角ゴシック';
  font-feature-settings: 'palt' 1;
  font-size: 32px;
  font-weight: 400;
  height: auto;
  letter-spacing: 0.1em;
  line-height: 1.5;
  margin: 120px 0 0 0;
  text-align: left;
  width: auto;
  max-width: 100%;
  justify-content: flex-start;
}

.h3-2{
  color: #FFFFFF;
  flex: none;
  font-family: '角ゴシック';
  font-feature-settings: 'palt' 1;
  font-size: 32px;
  font-weight: 400;
  height: auto;
  letter-spacing: 0.1em;
  line-height: 1.5;
  margin: 15px 0 0 0;
  text-align: left;
  width: auto;
  max-width: 100%;
  justify-content: flex-start;
}
.aboutContents {
  color: #FFFFFF;
  flex: none;
  font-family: '角ゴシック';
  font-feature-settings: 'palt' 1;
  font-size: 16px;
  font-weight: 400;
  height: auto;
  letter-spacing: 0.1em;
  line-height: 1.9;
  margin: 50px 0 0 0;
  text-align: left;
  width: 100%;
  max-width: 100%;
  justify-content: flex-start;
}

.readMore {
  align-content: center;
  align-items: center;
  flex: none;
  flex-direction: row;
  flex-wrap: nowrap;
  height: auto;
  justify-content: flex-end;
  margin: 60px 0 0 0;
  padding: 0 0 0 0;
  width: 100%;
  z-index: 0;
  max-width: 100%;
}

.aboutBackground {
  background: #f53c08;
  bottom: 0;
  flex: none;
  height: auto;
  left: 0;
  margin: 0 0 0 0;
  position: absolute;
  right: 0;
  top: 0;
  width: auto;
  z-index: -1;
  max-width: 100%;
}

.worksTitle {
  height: 60px;
  width: 100%;
  text-align: center;
  margin-bottom: 20px;
}

.worksContents {
  height: 450px;
  width: 700px;
  top: 0;
  right: 0;
  left: 0;
  bottom: 0;
  margin: auto;
}

.works {
  height: 800px;
  width: 100%;
  position: relative;
  padding-top: 250px;
}

.worksCard {
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  justify-content: space-between;
}

.card {
  width: 200px;
  height: 320px;
}

.card__imgframe {
  width: 100%;
  height: 125px;
  padding-top: 56.25%;
  background: url(https://placehold.jp/640x360.png) no-repeat center;
  background-size: cover;
  box-sizing: border-box;
}

.card__textbox {
  width: 100%;
  height: auto;
  padding: 20px 18px;
  background: #ffffff;
  box-sizing: border-box;
}

.card__textbox > * + * {
  margin-top: 10px;
}

.card__titletext {
  font-size: 20px;
  font-weight: bold;
  line-height: 125%;
}

.card__overviewtext {
  font-size: 12px;
  line-height: 150%;
}

.project {
  height: 1400px;
  width: 100%;
}

.projectTitle {
  height: 500px;
  width: 100%;
}

.projectText1 {
  height: 150px;
  width: auto;
}

.projectTexts {
  height: 235px;
  width: auto;
}

.projectTexts img {
  float: left;
}

.projectText2 {
  float: right;
}

.projectContents1 {
  height: 320px;
  width: 500px;
  position: relative;
  margin: 100px 0 0 auto;
}

.projectContents1 img {
  position: absolute;
  z-index: 1;
}

.projectTextbox1 {
  position: absolute;
  right: 0;
  bottom: 0;
  z-index: 2;
  height: 170px;
  width: 440px;
}

.projectContents2 {
  height: 320px;
  width: 500px;
  position: relative;
  margin-top: 65px;
}

.projectContents2 img {
  position: absolute;
  z-index: 1;
}

.projectTextbox2 {
  position: absolute;
  right: 0;
  bottom: 0;
  z-index: 2;
  height: 170px;
  width: 440px;
}

.image:before {
  content: "";
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  position: absolute;
  border-radius: inherit;
  z-index: -2;
  pointer-events: none;
  background-size: cover;
  background-position: 50%;
  transition: inherit;
}

</style>
