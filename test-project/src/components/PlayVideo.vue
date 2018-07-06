<template>
  <v-layout row wrap class="bg__play__video">
    <v-flex class="bg__gradient"></v-flex>
    <v-flex xs12 class="on__img">
      <v-flex xs12 sm8 md6 lg4 offset-sm2 offset-md3 offset-lg4 class="stl__text pt-5 pb-5">
        <h1>Watch <span>video tour</span></h1>
        <span class="pt-3 pb-3">This sounded nonsense to Alice, so she said nothing, but set off at once toward the Red Queen. To her surprise, she lost sight of her.</span>
        <div class="circle">
          <div>
            <div>
              <div class="circle__fa">
                <i class="fas fa-play"></i>
              </div>
            </div>
          </div>
        </div>
      </v-flex>
    </v-flex>
  </v-layout>
</template>

<script>
export default {
}
</script>

<style>
.bg__play__video {
  background-image: linear-gradient(135deg, #7956ec, #2fb9f8);
  height: 700px;
  position: relative;
}

.on__img {
  display: flex;
  align-content: center;
  z-index: 5;
}

.bg__gradient {
  opacity: 1;
  position: absolute;
  background-image: url(../assets/img/image.png);
  background-size: cover;
  background-position: center;
  width: 100%;
  height: 100%;
  background-repeat: no-repeat;
}

.circle {
  width: 130px;
  height: 130px;
  border-radius: 80px;
  border: 1px solid rgba(2555, 2555, 255, 0.1);
  display: flex;
  align-items: center;
  justify-content: center;
  margin-left: auto;
  margin-right: auto;
}

.circle > div {
  width: 85%;
  height: 85%;
  border-radius: 60px;
  border: 2px solid rgba(2555, 2555, 255, 0.3);
  display: flex;
  align-items: center;
  justify-content: center;
}

.circle > div > div {
  width: 85%;
  height: 85%;
  border-radius: 60px;
  border: 3px solid rgba(2555, 2555, 255, 0.5);
  display: flex;
  align-items: center;
  justify-content: center;
}

.circle__fa {
  width: 80%;
  height: 85%;
  border-radius: 60px;
  background-color: #ffffff;
  display: flex;
  align-items: center;
  justify-content: center;
}

.circle__fa > .fa-play:before {
  font-size: 26px;
  background: -webkit-gradient(linear, left top, left bottom, from( #ff8e64), to(#ffe641));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  display: initial;
}

.stl__text {
  justify-content: center;
  align-items: center;
  display: flex;
  flex-direction: column;
}

.stl__text > h1 {
  font-size: 35px;
  letter-spacing: normal;
  text-align: center;
  color: #ffffff;
  font-family: NunitoSans;
}

.stl__text > h1 > span {
  font-weight: 300;
}

.stl__text > span {
  font-size: 16px;
  font-family: NunitoSans;
  font-weight: normal;
  font-style: normal;
  font-stretch: normal;
  line-height: 1.88;
  letter-spacing: normal;
  text-align: center;
  display: block;
  color: rgba(255, 255, 255, 0.8);
}

.ild > .fa-inbox:before {
  font-size: 24px;
  background: -webkit-gradient(linear, left top, left bottom, from( #ff8e64), to(#ffe641));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  display: initial;
}
</style>
