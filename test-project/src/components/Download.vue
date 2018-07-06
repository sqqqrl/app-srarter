<template>
  <v-layout row wrap xs10 justify-space-between align-center offset-xs1 class="bg__theme">
    <v-flex xs10 md6 lg4 offset-xs1 class="mt-5 mb-5 download__title">
      <h1 class="pb-4">Download <span>to get started</span></h1>
      <span>This sounded nonsense to Alice, so she said nothing, but set off at once toward the Red Queen. To her surprise, she lost sight of her in a moment.</span>
    </v-flex>

    <v-flex xs10 md3 lg5 offset-xs1 class="column__adpt" justify-center>
      <v-btn class="btn__download__watch download pl-4 pr-4">Buy for $24</v-btn>
      <v-btn class="btn__download__watch white ml-4 pl-4 pr-4">Try It Free</v-btn>
    </v-flex>
  </v-layout>
</template>

<script>
export default {
}
</script>

<style>
.main__content > .bg__theme {
  margin-bottom: 0;
}

.download__title > h1{
  font-family: NunitoSans;
  font-size: 35px;
  letter-spacing: 0.9px;
  color: #ffffff;
}

.download__title > h1 > span {
  font-weight: 300;
}

.download__title > span {
  opacity: 0.8;
  font-family: NunitoSans;
  font-size: 16px;
  line-height: 1.88;
  letter-spacing: normal;
  color: rgba(255, 255, 255, 0.8);
}

@media (max-width: 480px){
  .btn__download__watch {
    margin-left: 0 !important;
    padding: 0 10px!important;
  }
}
</style>
