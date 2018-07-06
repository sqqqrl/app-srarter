<template>
  <v-layout row wrap xs8 lg10 align-center justify-center offset-xs2 class="white pt-5 pb-5">
    <v-flex xs5 sm4 md2 xl1 class="mr-3 no__pm">
      <img src="../assets/img/wired.png" alt="">
    </v-flex>
    <v-flex xs5 sm4 md2 xl1 class="mr-3 no__pm">
      <img src="../assets/img/lifehacker.png" alt="">
    </v-flex>
    <v-flex xs5 sm4 md2 xl1 class="mr-3 no__pm">
      <img src="../assets/img/mashable.png" alt="">
    </v-flex>
    <v-flex xs5 sm4 md2 xl1 class="fullsize__img mr-3 no__pm">
      <img src="../assets/img/images.jpeg" alt="">
    </v-flex>
    <v-flex xs5 sm4 md2 xl1 class="mr-3 no__pm">
      <img src="../assets/img/gizmodo.png" alt="">
    </v-flex>
    <v-flex xs5 sm4 md2 xl1 class="mr-3 no__pm">
      <img src="../assets/img/macworld.png" alt="">
    </v-flex>
  </v-layout>
</template>

<script>
export default {
}
</script>

<style>
.fullsize__img > img {
  width: 100%;
}
@media (max-width: 1904px){
  .no__pm {
    margin-right: 0 !important;
    text-align: center;
  }
}
</style>
