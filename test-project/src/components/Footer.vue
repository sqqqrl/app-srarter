<template>
  <v-layout row wrap xs12 class="white footer">
    <v-flex xs10 offset-xs1>
      <v-layout row wrap xs12 justify-space-between>
        <v-flex xs6 sm4 lg2 class="footer__title d-flex align-center">
          <h1>AppStarter</h1>
        </v-flex>
        <v-flex xs12 order-xs2 sm4 lg2 class="middle__text d-flex align-center">
          <span>Created with <i class="fas fa-heart"></i> by <b>Sergey Azovskiy</b></span>
        </v-flex>
        <v-flex xs6 sm4 order-sm3 lg2 class="d-flex align-center justify-center">
          <i class="coube__border fab fa-twitter"></i>
          <i class="coube__border fab fa-facebook-f"></i>
          <i class="coube__border fab fa-instagram"></i>
        </v-flex>
      </v-layout>
      <v-layout row wrap xs12 justify-center>
        <v-flex class="copyright d-flex align-center">
          <span>&#9400; AppStarter, 2017</span>
        </v-flex>
      </v-layout>
    </v-flex>
  </v-layout>
</template>

<script>
export default {
}
</script>

<style>
.footer__title > h1 {
  font-family: NunitoSans;
  font-size: 20px;
  font-weight: 800;
  font-style: normal;
  font-stretch: normal;
  letter-spacing: normal;
  color: #282b31;
}

.coube__border {
  max-width: 40px;
  height: 40px;
  background-color: #ffffff;
  border: solid 1px #e7e8ea;
  font-size: 20px;
  color: #999ea8;
  display: flex;
  align-items: center;
  justify-content: center;
  box-shadow: inset 0px 1px 0 0 #e7e8ea, inset 0px -1px 0 0 #e7e8ea;
}

.coube__border:nth-child(1) {
  border-radius: 5px 0 0 5px;
}

.coube__border:nth-child(3) {
  border-radius: 0 5px 5px 0;
}

.footer {
  height: 110px;
}

.middle__text > span {
  font-family: NunitoSans;
  font-size: 11px;
  font-weight: normal;
  font-style: normal;
  font-stretch: normal;
  letter-spacing: normal;
  text-align: center;
  color: rgba(153, 158, 168, 0.8)
}

.middle__text > span > i {
  color: #ff4876;
}

.middle__text > span > b {
  font-weight: 800;
  color: rgba(0, 0, 0, 1)
}

.copyright {
  font-family: NunitoSans;
  font-size: 11px;
  font-weight: normal;
  font-style: normal;
  font-stretch: normal;
  letter-spacing: normal;
  text-align: center;
  color: #999ea8;
}
</style>
