<template>
<v-layout xs10 offset-xs1 row wrap class="mb-5__adapt">
  <v-flex xs10 offset-xs1 lg5 offset-lg0 class="vh__center vh__adpt">
    <v-flex xs12 lg7 class="choose__text">
      <h1>Choose <span>your plan</span></h1>
      <span>This sounded nonsense to Alice, so she said nothing, but set off at once toward the Red Queen. To her surprise, she lost sight of her in a moment, and found herself walking.</span>
    </v-flex>
  </v-flex>
  <v-flex xs12 sm10 offset-sm1 lg7 offset-lg0 class="second__tab">
    <v-flex xs10 sm6 lg5 class="tab__plan">
      <div class="opacity__bg mb-5 pt-5">
        <h3 class="pt-2 pb-2 d-flex align-center justify-center">Professional</h3>
        <span></span>
      </div>
      <span class="mb-5">10$</span>
      <v-flex xs8 lg8 offset-xs2 offset-lg2 class="ul__btn li_white">
        <ul>
          <li>Hundreds of elements</li>
          <li>Style guide</li>
          <li>160 icons included</li>
          <li>Sketch files</li>
          <li>Commercial licence</li>
        </ul>
      <v-btn class="download buy__now mt-5 mb-5">Buy Now</v-btn>
      </v-flex>
    </v-flex>
    <v-flex xs10 sm6 lg5 class="white tab__full__stl">
      <div class="opacity__bg2 mb-5 pt-5">
        <h3 class="pt-2 pb-2 d-flex align-center justify-center">Starter</h3>
        <span></span>
      </div>
      <span class="mb-5">FREE</span>
      <v-flex xs8 lg8 offset-xs2 offset-lg2 class="ul__btn li_grey">
        <ul>
          <li>Hundreds of elements</li>
          <li>Style guide</li>
          <li>30 icons included</li>
          <li>Personal licence</li>
        </ul>
        <v-btn class="get__free buy__now mt-5 mb-5">Get Free</v-btn>
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
.choose__text > h1{
  font-family: NunitoSans;
  font-size: 35px;
  font-style: normal;
  font-stretch: normal;
  line-height: 2.5;
  letter-spacing: 0.9px;
  text-align: left;
  color: #282b31;
}

.choose__text > h1 > span {
  font-weight: 300;
}

.choose__text > span {
  font-family: NunitoSans;
  font-size: 16px;
  font-weight: normal;
  font-style: normal;
  font-stretch: normal;
  line-height: 1.88;
  letter-spacing: normal;
  text-align: left;
  color: #676c75;
}

.choose__text {
  justify-content: center;
  display: flex;
  flex-direction: column;
}

.tab__plan {
  background-image: url('../assets/img/bg1.png');
  background-repeat: no-repeat;
  background-size: 100% 100%;
  border-radius: 20px;
}

.opacity__bg > h3 {
  font-family: NunitoSans;
  font-size: 11px;
  font-weight: 800;
  font-style: normal;
  font-stretch: normal;
  line-height: 1.36;
  letter-spacing: 1.7px;
  text-align: center;
  color: #ffffff;
  text-transform: uppercase;
  height: 39px;
  border: 1px solid rgba(255, 255, 255, 0.3);
}

.opacity__bg2 > h3 {
  font-family: NunitoSans;
  font-size: 11px;
  font-weight: 800;
  font-style: normal;
  font-stretch: normal;
  line-height: 1.36;
  letter-spacing: 1.7px;
  text-align: center;
  color: #676c75;
  text-transform: uppercase;
  height: 39px;
  border: 1px solid rgba(255, 255, 255, 0.3);
}

.opacity__bg {
  position: relative;
}

.opacity__bg2 {
  position: relative;
}

.opacity__bg > h3:before {
  content: "";
  width: 100%;
  display: block;
  height: 39px;
  background-color: #f8f9fa;
  opacity: 0.2;
  position: absolute;
  box-shadow: 0px 1px 0 0 rgba(255, 255, 255, 0.3), inset 0px 1px 0 0 rgba(255, 255, 255, 0.3);
}

.opacity__bg2 > h3:before {
  content: "";
  width: 100%;
  display: block;
  height: 39px;
  background-color: #aaaaaa;
  opacity: 0.2;
  position: absolute;
  box-shadow: 0px 1px 0 0 rgba(255, 255, 255, 0.3), inset 0px 1px 0 0 rgba(255, 255, 255, 0.3);
}

.tab__plan > span {
  display: block;
  width: 100%;
  font-family: NunitoSans;
  font-size: 60px;
  font-weight: 300;
  font-style: normal;
  font-stretch: normal;
  line-height: 1.37;
  letter-spacing: normal;
  text-align: center;
  color: #ffffff;
}

.ul__btn > ul > li {
  list-style: none;
  font-family: NunitoSans;
  font-size: 15px;
  font-weight: normal;
  font-style: normal;
  font-stretch: normal;
  line-height: 1.5;
  letter-spacing: normal;
  text-align: left;
}

.li_white > ul > li {
  color: #ffffff;
}

.li_grey > ul > li {
  color: #676c75;;
}

.ul__btn > ul > li::before {
  content: '\f00c';
  font-family: FontAwesome;
  font-size: 18px;
  margin-right: 10px;
}

.buy__now {
  border-radius: 6px;
  width: 100%;
  height: 50px;
  font-family: NunitoSans;
  font-size: 17px;
  font-weight: bold;
  font-style: normal;
  font-stretch: normal;
  letter-spacing: 0.9px;
  color: #ffffff;
  text-transform: none;
  margin: 0;
}

.get__free {
  background-image: linear-gradient(135deg, #009fc5, #3cecb0);
  box-shadow: 0px 6px 12px 0 rgba(40, 43, 49, 0.08);
  border-radius: 6px;
}

.second__tab {
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-items: center;
}

.tab__full__stl {
  border-radius: 0 15px 15px 0;
}

.tab__full__stl > span {
  display: block;
  width: 100%;
  font-family: NunitoSans;
  font-size: 40px;
  font-weight: 300;
  font-style: normal;
  font-stretch: normal;
  line-height: 1.35;
  letter-spacing: normal;
  text-align: center;
  color: #282b31;
}

@media (max-width: 660px) {
  .tab__full__stl {
    margin-top: 15px;
    border-radius: 15px;
  }
}

@media (max-width: 1263px) {
  .vh__adpt{
    height: auto;
    margin-bottom: 50px;
  }
  .mb-5__adapt {
    margin-bottom: 50px;;
  }
}
</style>
