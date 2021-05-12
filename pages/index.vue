<template>
  <div class="container sd">
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
      <div class="aboutSpace"></div>
      <div class="image1">
        <div class="aboutImg1">

        </div>
      </div>
      <div class="aboutContents">
        <h2 class="text ">about</h2>
        <h3 class="text h3-1">”ゆれる”を創る</h3>
        <h3 class="text h3-2">それをココから。</h3>
        <p class="textP">
          何か、なだらかなアシタに昨日の香りを感じる、今日このごろ。
          <br>
          今日より、明日がよくなるとお思いですか？
          <br>
          意外と変わりませんよ。明日も今日も。
        </p>
        <div class="readMore">
          <a href="index.vue" class="readLink">
            <div class="aboutLine"></div>
            <p class="readText">Read More</p>
          </a>
        </div>
        <div class="aboutBackground"></div>
      </div>

      <div class="aboutImgs">
        <div class="image2">
        </div>
        <div class="image3">
        </div>
      </div>
      <div class="aboutSpace1"></div>
    </div>
    <div class="works">
      <div class="worksText sd">
        <h2 class="h2-2">works</h2>
      </div>
      <div class="worksContent1">
        <div class="worksImg1 sd"></div>
        <div class="worksText1">
          <h3 class="h3-3">ショウ、チク、バイ<br>にほんのカタチ</h3>
          <p class="worksTextP">いつかの明日は、今日の一瞬。<br>
            忘れないよう、メモに書いた、<br>
            消えていく日本のカタチ、<br>
            僕は何も知らない。</p>
        </div>
      </div>
      <div class="worksContent2">
        <div class="worksSpace"></div>
        <div class="worksText2">
          <h3 class="h3-4">
            クリームソーダーを飲んだ、<br>
            あのときの記憶。</h3>
          <p class="worksTextP2">忘れていくのは、当然のこと。だけど、伝えて
            いくことは僕らの役割。</p>
        </div>
        <div class="worksSpace"></div>
        <div class="worksImg2 sd"></div>
      </div>
      <div class="worksContent3">
        <div class="worksImg3"></div>
        <div class="worksText3">
          <div class="h3-5">夢にみたインド<br>
            サクッと話すには荷が重い
          </div>
          <div class="worksTextP3">友達が飼ってたブラウンのプードル、家で啜った<br>
            昨日のヌードル、それでキンドル眺めればサクッと<br>
            荷が重い話の完成。
          </div>
        </div>
      </div>
    </div>

    <div class="project sd">
      <div class="projectNoren sd">
        <img src="../static/sample.jpg" class="noren">
      </div>
      <div class="projectContents sd">
        <div class="projectText">
          <h2 class="h2-3">project</h2>
        </div>
        <div class="projectContent2">
          <div class="projectRadius sd">
            <img src="../static/sample.jpg" class="radius">
            <h3 class="radiusText">キノウ</h3>
          </div>
          <div class="projectRadius sd">
            <img src="../static/sample.jpg" class="radius">
            <h3 class="radiusText">イマ</h3>
          </div>
          <div class="projectRadius sd">
            <img src="../static/sample.jpg" class="radius">
            <h3 class="radiusText">アシタ</h3>
          </div>
        </div>
      </div>
      <div class="projectBackground"></div>
    </div>
    <div class="projectText2">
      <div class="projecttextContents"><img class="projectImg" src="../static/sample.jpg"></div>
      <div class="projecttextContents"><img class="projectImg" src="../static/sample.jpg"></div>
      <div class="projecttextContents"><img class="projectImg" src="../static/sample.jpg"></div>
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
  display: flex;
  position: relative;
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

.h3-1 {
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

.h3-2 {
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

.textP {
  color: #FFFFFF;
  flex: none;
  font-family: '角ゴシック';
  font-feature-settings: 'palt' 1;
  font-size: 16px;
  font-weight: 400;
  height: auto;
  letter-spacing: 0.1em;
  line-height: 1.9;
  margin: 50px 0px 0px 0px;
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
  display: flex;
  position: relative;
}

.readLink {
  align-content: center;
  align-items: center;
  flex-direction: row;
  flex-wrap: nowrap;
  justify-content: center;
  padding: 5px 0px 5px 0px;
  z-index: 0;
  display: flex;
  text-decoration: none;
}

.readText {
  color: #FFFFFF;
  flex: none;
  font-family: Helvetica;
  font-size: 18px;
  font-weight: 600;
  height: auto;
  letter-spacing: 0.1em;
  line-height: 1.4;
  text-align: right;
  width: auto;
  max-width: 100%;
  justify-content: flex-end;
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

.aboutSpace {
  align-content: center;
  align-items: center;
  background: #FFFFFF;
  flex: none;
  flex-direction: column;
  flex-wrap: nowrap;
  height: 100px;
  justify-content: center;
  width: 100%;
  z-index: 0;
  max-width: 100%;
}

.aboutImg1 {
  flex: none;
  height: 70vh;
  width: 90%;
  max-width: 90%;
  position: relative;
  z-index: 1;
}

.aboutImg1:before {
  content: ''; /*何も入れない*/
  display: inline-block; /*忘れずに！*/
  width: 100%; /*画像の幅*/
  height: 100%; /*画像の高さ*/
  background-image: url(../static/sample.jpg);
  background-size: cover;
  vertical-align: middle;
}

.image1 {
  align-content: flex-start;
  align-items: flex-start;
  flex-direction: row;
  flex-wrap: nowrap;
  justify-content: flex-start;
  margin: -100px 0 0 0;
  padding: 0;
  width: 100%;
  max-width: 100%;
  display: flex;
  position: relative;
  z-index: 0;
}

.aboutLine {
  align-content: flex-start;
  align-items: flex-start;
  background: #FFFFFF;
  flex: none;
  flex-direction: column;
  flex-wrap: nowrap;
  height: 1px;
  justify-content: center;
  margin: 0px 20px 0px 0px;
  opacity: 0.7;
  width: 80px;
  max-width: calc(100% - 20px);
}

.aboutImgs {
  align-items: flex-end;
  background: rgba(0, 0, 0, 0.0);
  flex: none;
  flex-direction: row;
  flex-wrap: nowrap;
  height: auto;
  justify-content: space-between;
  margin: 60px 0px 0px 0px;
  padding: 0px;
  transform: translate(0px, 0px);
  width: 100%;
  z-index: 1;
  max-width: 100%;
  position: relative;
  display: flex;
}

.image2 {
  flex: none;
  height: 55vh;
  margin: 0px 0px 100px 0px;
  width: 45%;
  max-width: 45%;
  align-content: center;
  align-items: center;
  flex-direction: column;
  flex-wrap: nowrap;
  justify-content: center;
}

.image2:before {
  content: ''; /*何も入れない*/
  display: inline-block; /*忘れずに！*/
  width: 100%; /*画像の幅*/
  height: 100%; /*画像の高さ*/
  background-image: url(../static/sample.jpg);
  background-size: cover;
  vertical-align: middle;
}

.image3 {
  flex: none;
  height: 55vh;
  width: 58%;
  max-width: 58%;
  margin: 0px 0px 0px -60px;
  padding: 0px 0px 0px 0px;
}

.image3:before {
  content: ''; /*何も入れない*/
  display: inline-block; /*忘れずに！*/
  width: 100%; /*画像の幅*/
  height: 100%; /*画像の高さ*/
  background-image: url(../static/sample.jpg);
  background-size: cover;
  vertical-align: middle;
}

.aboutSpace1 {
  flex: none;
  height: 100px;
  margin: -100px 0px 0px 0px;
  width: 100%;
  max-width: 100%;
  z-index: 0;
  background-color: #FFFFFF;
}

.works {
  height: auto;
  width: 100%;
  position: relative;
}

.worksText {
  margin: 160px 0 100px 0;
  justify-content: center;
  height: auto;
  width: 100%;
  padding: 0;
}

.h2-2 {
  font-family: 角ゴシック;
  font-size: 64px;
  word-spacing: 70px;
  font-weight: bold;
}

.worksContent1 {
  height: 100%;
  width: 90%;
  min-width: 90%;
  margin: 100px 0 0 0;
  justify-content: space-between;
  flex-direction: row;
  display: flex;
  align-content: center;
  align-items: center;
}

.worksTextP {
  align-items: flex-start;
  align-content: flex-start;
  justify-content: flex-start;
  height: auto;
  margin: 30px 0;
}

.worksText1 {
  align-items: center;
  align-content: center;
  justify-content: flex-start;
  width: 38%;
  min-width: 38%;
  height: auto;
  flex: none;
  flex-direction: column;
  flex-wrap: nowrap;
}

.worksImg1 {
  height: 50vh;
  width: 55%;
  min-width: 55%;
}

.worksImg1:before {
  content: ''; /*何も入れない*/
  display: inline-block; /*忘れずに！*/
  width: 100%; /*画像の幅*/
  height: 100%; /*画像の高さ*/
  background-image: url(../static/sample.jpg);
  background-size: cover;
  vertical-align: middle;
}

.h3-3 {
  font-size: 24px;
  font-family: 角ゴシック;
  align-items: flex-start;
  align-content: flex-start;
  justify-content: flex-start;
}

.worksContent2 {
  height: auto;
  width: 80%;
  min-width: 80%;
  margin: 120px 0 0 0;
  flex-direction: row;
  justify-content: flex-end;
  display: flex;
}

.worksText2 {
  width: 45%;
  align-content: flex-start;
  align-items: flex-start;
  justify-content: flex-start;
  flex-grow: 0;
}

.worksTextP2 {
  font-family: 角ゴシック;
  font-size: 16px;
  margin-top: 30px;
}

.h3-4 {
  font-family: 角ゴシック;
  font-size: 24px;
  font-weight: bold;
}

.worksImg2 {
  width: 40%;
  height: 80vh;
  flex-grow: 0;
}

.worksImg2:before {
  content: ''; /*何も入れない*/
  display: inline-block; /*忘れずに！*/
  width: 100%; /*画像の幅*/
  height: 100%; /*画像の高さ*/
  background-image: url(../static/sample2.jpg);
  background-size: cover;
  vertical-align: middle;
}

.worksSpace {
  width: 7.5%;
  height: 50px;
  flex-grow: 0;
}

.worksContent3 {
  height: auto;
  width: 80%;
  min-width: 80%;
  justify-content: space-between;
  flex-direction: row;
  display: flex;
  align-content: flex-end;
  align-items: flex-end;
  margin: -160px 0 0 0;
}

.worksText3 {
  width: 45%;
  align-content: flex-start;
  align-items: flex-start;
  justify-content: flex-start;
}

.h3-5 {
  font-size: 24px;
  font-family: 角ゴシック;
  font-weight: bold;
}

.worksTextP3 {
  font-size: 16px;
  font-family: 角ゴシック;
  margin-top: 30px;
}

.worksImg3 {
  width: 40%;
  height: 80vh;
  flex-grow: 0;
}

.worksImg3:before {
  content: ''; /*何も入れない*/
  display: inline-block; /*忘れずに！*/
  width: 100%; /*画像の幅*/
  height: 100%; /*画像の高さ*/
  background-image: url(../static/sample2.jpg);
  background-size: cover;
  vertical-align: middle;
}

.project {
  width: 100%;
  height: auto;
  position: relative;
  margin-top: 160px;
}

.projectNoren {
  width: 100%;
  height: 100vh;

}

.noren {
  width: 100%;
  height: 100%;
  background-size: cover;
}

.projectText {
  width: 100%;
  height: auto;
  display: flex;
  align-items: center;
  align-content: center;
  justify-content: center;
}

.projectContents {
  width: 100%;
  height: auto;
  margin-top: 160px;
}

.h2-3 {
  font-size: 64px;
  font-family: Helvetica;
  color: #FFFFFF;
}

.projectContent2 {
  margin: 140px 0 0 0;
  display: flex;
  align-content: space-between;
  justify-content: space-between;
  flex: none;
  flex-direction: row;
  width: 75%;
  height: auto;
}

.radius {
  border-radius: 50%;
  height: 250px;
  width: 250px;
}

.radiusText {
  font-family: 角ゴシック;
  font-size: 28px;
  margin-top: 35px;
  color: #FFFFFF;
}

.projectRadius {
  margin: 0 0 100px 0;
}

.projectBackground {
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

.projectText2{
  margin: -50px 0 0 0;
  height: 400px;
  width: 75%;
  display: flex;
  flex-direction: row;
  position: relative;
  justify-content: space-between;
}

.projecttextContents{
  height: 400px;
  width: 235px;
  background-color: #FFFFFF;
  display: flex;
  justify-content: center;
  box-shadow: 2px 2px 8px 0.5px black ;
}

.projectImg{
  height: 180px;
  width: 235px;
}

.sd {
  max-width: 100%;
  z-index: 0;
  pointer-events: all;
  flex-wrap: nowrap;
  -webkit-overflow-scrolling: touch;
  display: flex;
  position: relative;
  flex-direction: column;
  align-content: center;
  align-items: center;
  flex: none;
}
</style>
