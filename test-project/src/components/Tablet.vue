<template>
  <v-layout row wrap xs8 align-center justify-center offset-xs2 class="pt-5 pb-5">
    <v-flex xs12 lg5>
      <v-flex xs12 sm8 md7 lg12 offset-sm2 class="mb-3 pa-4">
        <v-layout row class="different__grd">
          <v-flex class="grd__div ild" xs2 sm1>
            <i class="fas fa-sync"></i>
          </v-flex>
          <v-flex class="stl__h2" xs10 sm11>
            <h2>Sync <span>across all devices</span></h2>
            <span>
              This sounded nonsense to Alice, so she said nothing, but set off at once toward the Red Queen. To her surprise, she lost sight of her in a moment.            </span>
          </v-flex>
        </v-layout>
      </v-flex>

      <v-flex xs12 sm8 md7 lg12 offset-sm2 class="mb-3 white pa-4 middle__box">
        <v-layout row class="different__grd">
          <v-flex class="grd__div ild" xs2 sm1>
            <i class="fas fa-inbox"></i>
          </v-flex>
          <v-flex class="stl__h2" xs10 sm11>
            <h2>All emails <span>in one place</span></h2>
            <span>
              This sounded nonsense to Alice, so she said nothing, but set off at once toward the Red Queen. To her surprise, she lost sight of her in a moment.            </span>
          </v-flex>
        </v-layout>
      </v-flex>

      <v-flex xs12 sm8 md7 lg12 offset-sm2 class="mb-3 pa-4">
        <v-layout row class="different__grd">
          <v-flex class="grd__div ild" xs2 sm1>
            <i class="far fa-clock"></i>
          </v-flex>
          <v-flex class="stl__h2" xs10 sm11>
            <h2>Notifications <span>about sales</span></h2>
            <span>
              This sounded nonsense to Alice, so she said nothing, but set off at once toward the Red Queen. To her surprise, she lost sight of her in a moment.            </span>
          </v-flex>
        </v-layout>
      </v-flex>
    </v-flex>
    <v-flex class="hidden__img" xs12 lg5 hidden-sm-and-down>
      <img src="../assets/img/tablet2.png" alt="">
    </v-flex>
  </v-layout>
</template>

<script>
export default {
}
</script>

<style>
.ild > .fa-sync:before  {
  font-size: 24px;
  background: -webkit-gradient(linear, left top, left bottom, from( #7956ec), to(#2fb9f8));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  display: initial;
}

.ild > .fa-inbox:before {
  font-size: 24px;
  background: -webkit-gradient(linear, left top, left bottom, from( #ff8e64), to(#ffe641));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  display: initial;
}

.ild > .fa-clock:before {
  font-size: 24px;
  background: -webkit-gradient(linear, left top, left bottom, from( #009fc5), to(#3cecb0));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  display: initial;
}

.stl__h2 > h2 {
  margin: 0 0 20px 0;
  font-family: NunitoSans;
  font-size: 20px;
  color: #282b31;
}

.stl__h2 > h2 > span {
  font-weight: 300;
}

.stl__h2 > span {
  font-family: NunitoSans;
  font-size: 14px;
  letter-spacing: normal;
  text-align: justify;
  display: block;
  color: #676c75;
  line-height: 1.79;
}

.middle__box {
  border-radius: 12px;
  box-shadow: 0px 6px 12px 0 rgba(32, 33, 39, 0.08);
}

@media (min-width: 960px) {
  .hidden__img {
    text-align: center;
  }
}
</style>
