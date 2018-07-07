<template>
  <v-layout id="reviewTarget" row wrap>
    <v-flex xs12 md4 lg4 class="white around__flex">
      <v-flex xs10  lg6 offset-xs1 offset-lg3 class="asd">
        <div class="customers">
          <img src="../assets/img/stars.png" alt="">
          <h1>Customers <span>about AppStarter</span></h1>
        </div>
      </v-flex>
      <v-flex xs10 lg6 offset-xs1 offset-lg3 class="reviews">
        <span>Read more reviews:</span>
        <div>
          <i class="fas fa-long-arrow-alt-right"></i>
          <a href="#">App Store</a>
        </div>
        <div>
          <i class="fas fa-long-arrow-alt-right"></i>
          <a href="#">Google Play</a>
        </div>
      </v-flex>
    </v-flex>
    <v-flex xs12 md8 lg8 class="vh__center mr__adapt">
      <v-flex xs12 md10 lg8>
        <v-flex xs11 md10 lg10 class="white customer__tab pa-4">
          <div class="d-flex customer__info">
            <img src="../assets/img/face1.png" alt="" class="ma-3">
            <span>This sounded nonsense to Alice, so she said nothing, but set off at once toward the Red Queen. To her surprise, she lost sight of her in a moment, and found herself.</span>
          </div>
          <div class="under__line">
            <span><b>Eliza Paul</b> - Web Designer</span>
            <i class="fab fa-twitter"></i>
          </div>
        </v-flex>

        <v-flex xs11 md10 lg10 class="white customer__tab pa-4 mt-4 mb-4">
          <div class="d-flex customer__info">
            <img src="../assets/img/face2.png" alt="" class="ma-3">
            <span>This sounded nonsense to Alice, so she said nothing, but set off at once toward the Red Queen. To her surprise, she lost sight of her in a moment, and found herself.</span>
          </div>
          <div class="under__line">
            <span><b>Juan Richards</b> - Photographer</span>
            <i class="fab fa-twitter"></i>
          </div>
        </v-flex>

        <v-flex xs11 md10 lg10 class="white customer__tab pa-4">
          <div class="d-flex customer__info">
            <img src="../assets/img/face1.png" alt="" class="ma-3">
            <span>This sounded nonsense to Alice, so she said nothing, but set off at once toward the Red Queen. To her surprise, she lost sight of her in a moment, and found herself.</span>
          </div>
          <div class="under__line">
            <span><b>Marian McGuire</b> - Entrepreneur</span>
            <i class="fab fa-twitter"></i>
          </div>
        </v-flex>
      </v-flex>
    </v-flex>
  </v-layout>
</template>

<script>
export default {
}
</script>

<style>
.vh__center {
  height: 100vh;
  display: flex;
  flex-flow: column;
  justify-content: center;
  align-items: center;
}

.customers > h1 {
  font-family: NunitoSans;
  font-size: 35px;
  font-style: normal;
  font-stretch: normal;
  line-height: 1.43;
  letter-spacing: 0.9px;
  text-align: left;
  color: #282b31;
}

.customers > h1 > span {
  font-weight: 300;
}

.reviews {
  font-family: NunitoSans;
  font-size: 15px;
  font-weight: bold;
  font-style: normal;
  font-stretch: normal;
  letter-spacing: 0.3px;
  text-align: left;
  color: #999ea8;
  display: flex;
  justify-content: center;
  flex-flow: column;
}

.reviews div {
  display: flex;
  align-items: center;
  margin: 15px 0;
}

.reviews div a {
  font-family: NunitoSans;
  font-size: 15px;
  font-weight: 800;
  font-style: normal;
  font-stretch: normal;
  letter-spacing: 0.6px;
  text-align: left;
  color: #282b31;
  text-decoration: none;
  margin: 0 5px;
}
.reviews div i {
  font-size: 20px;
}

.around__flex {
  display: flex;
  flex-direction: column;
  justify-content: space-around;
  align-content: center;
}

.asd {
  display: flex;
  align-items: center;
  justify-content: center;
}

.customer__tab {
  max-height: 180px;
  border-radius: 20px;
  display: flex;
  flex-flow: column;
  justify-content: space-between;
}

.customer__info img {
  border-radius: 30px;
  max-width: 50px;
  max-height: 50px;
}
.customer__info > span {
  font-family: NunitoSans;
  font-size: 14px;
  font-weight: normal;
  font-style: italic;
  font-stretch: normal;
  line-height: 1.79;
  letter-spacing: normal;
  text-align: left;
  color: #282b31;
  margin: 4px;
}

.customer__info {
  padding-bottom: 20px;
  border-bottom: 1px solid #e7e8ea;
}

.under__line > span {
  font-family: NunitoSans;
  font-size: 12px;
  font-weight: normal;
  font-style: normal;
  font-stretch: normal;
  line-height: 2.08;
  letter-spacing: normal;
  text-align: left;
  color: #999ea8;
}

.under__line {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.under__line > i {
  font-size: 20px;
  color: #d3d5d9;
}

.customer__tab:nth-child(2) {
  margin-left: auto;
}

@media (max-width: 1100px){
  .customer__tab {
    margin-left: auto;
    margin-right: auto;
    max-height: 230px;
  }
  .mr__adapt {
    margin-top: 20px;
  }
}

@media (min-width: 960px) and (max-width: 1100px){
  .customer__tab:nth-child(2) {
    margin-right: 0;
  }
}
</style>
