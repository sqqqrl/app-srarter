<template>
  <v-layout row wrap justify-center align-center>
    <v-container xs12 class="none__pm__b">
      <v-layout row wrap justify-center>
        <v-flex xs12 md6 lg5 class="bg__without__margin chess__tab" >
          <img src="../assets/img/tablet3.png" alt="">
        </v-flex>
        <v-flex xs12 md6 lg5 class="white all__chess">
          <v-flex xs10 offset-xs1  lg6 offset-lg3 class="tab__text all__chess">
            <h1>Perfect <span>landing page for your app</span></h1>
            <span>
              This sounded nonsense to Alice, so she said nothing, but set off at once toward the Red Queen. To her surprise, she lost sight of her in a moment, and found herself walking.
            </span>
          </v-flex>
        </v-flex>
      </v-layout>
    </v-container>
    <v-container class="none__pm__t" xs12>
      <v-layout row wrap justify-center>
        <v-flex xs12 md6 order-xs2 lg5 class="white all__chess">
          <v-flex xs10 offset-xs1 lg6 offset-lg3 class="tab__text all__chess">
            <h1>Style guide  <span>and sample pages included</span></h1>
            <span>
              This sounded nonsense to Alice, so she said nothing, but set off at once toward the Red Queen. To her surprise, she lost sight of her in a moment, and found herself walking.
            </span>
          </v-flex>
        </v-flex>
        <v-flex xs12 order-md2 md6 lg5 class="bg__without__margin chess__tab" >
          <img src="../assets/img/tablet4.png" alt="">
        </v-flex>
      </v-layout>
    </v-container>
  </v-layout>
</template>

<script>
export default {
}
</script>

<style>
.chess__tab {
  background-size: cover;
  text-align: center;
}
.chess__tab > img {
  padding: 50px 0 0 0;
  margin-bottom: -4px;
}

.tab__text > h1{
  font-family: NunitoSans;
  font-size: 35px;
  line-height: 1.43;
  text-align: center;
  color: #282b31;
}

.tab__text > h1 > span {
  font-weight: 300;
}

.tab__text > span {
  font-family: NunitoSans;
  font-size: 16px;
  line-height: 1.88;
  text-align: center;
  display: block;
  color: #676c75;
}

.all__chess {
  display: flex;
  flex-direction: column;
  align-content: center;
  justify-content: center;;
}

.bg__without__margin {
  background-image: url('../assets/img/bg1.png');
  background-repeat: no-repeat;
  padding-top: 50px;
}

.none__pm__t {
  padding-top: 0;
  margin-top: 0;
}

.none__pm__b {
  padding-bottom: 0;
  margin-bottom: 0;
}

@media (max-width: 700px){
  .chess__tab > img {
    width: 80%;
    padding-top: 0;
  }
}
</style>
