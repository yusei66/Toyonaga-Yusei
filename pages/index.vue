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
      <img src="../static/sample01.jpg" class="aboutImg1" height="550px" width="880px"/>
      <div class="aboutContents">
        <h1>about</h1>
        <p class="mainText">こんにちは。今日は、いい天気ですね。</p>
      </div>
      <div class="aboutBackground">
        画像
      </div>
      <img src="../static/sample02.jpg" class="aboutImg2" height="400px" width="600px"/>
      <img src="../static/sample03.jpg" class="aboutImg3" height="400px" width="600px"/>
    </div>
    <div class="works">

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

.aboutBackground {
  margin-top: 100px;
  height: 1000px;
  width: 100%;
  background-color: #35495e !important;
  z-index: 1;
  position: absolute;
}

.p {
  font-size: 16px;
  z-index: 3;

}

.about {
  height: 1500px;
  width: 100%;
  position: relative;
}

.aboutContents {
  position: absolute;
  z-index: 2;
  height: 550px;
  width: 100%;
  top: 550px;
}

.works {
  height: 1300px;
  width: 100%;
  position: relative;
}

.aboutImg1 {
  position: absolute;
  z-index: 2;
}

.aboutImg2{
  position: absolute;
  top: 1100px;
  left: 200px;
}

.aboutImg3{
  position: absolute;
  top: 1165px;
  right: 200px;
}

</style>
