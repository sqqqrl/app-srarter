<template>
  <v-layout column>
    <v-menu bottom left>
        <v-btn
          slot="activator"
          dark
          icon
        >
          <v-toolbar-side-icon v-on:click="click"></v-toolbar-side-icon>
        </v-btn>

        <v-list>
          <v-list-tile
            v-for="(item, index) in items"
            :key="index">
            <a class="group__btn" v-scroll-to="`${item.target}`" href="#">{{ item.title }}</a>
          </v-list-tile>
        </v-list>
      </v-menu>
    <v-toolbar  flat dark class="hidden-sm-and-down ovr__hd">
      <v-toolbar-title>AppStarter</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="align-center none__case"
        v-for="(item, index) in items"
        :key="index">
        <v-btn class="mr-3" v-scroll-to="`${item.target}`" flat>{{ item.title }}</v-btn>
      </v-toolbar-items>
      <v-toolbar-side-icon v-on:click="click"></v-toolbar-side-icon>
    </v-toolbar>
    <v-container fluid grid-list-md >
      <v-layout row wrap align-center class="adaptive__space__between">
        <v-flex xs12 sm10 md5 xl4>
          <img src="../assets/img/app-icon.png" alt="">
          <br>
          <h1 id="mainTitle">AppStarter. <span> Best landing page for web and mobile apps </span> </h1>
          <v-btn class="btn__download__watch download">Download Now</v-btn>
          <v-btn class="btn__download__watch white ml-2">Watch Video</v-btn>
        </v-flex>
        <v-flex xs12 md4 xl6 offset-xs1 class="hidden-sm-and-down alg__img">
          <img src="../assets/img/tablet.png" alt="">
        </v-flex>
      </v-layout>
    </v-container>
  </v-layout>
</template>

<script>
export default {
  data: () => ({
    items: [
      {
        title: 'Features',
        target: '#featuresTarget'
      },
      {
        title: 'Video Tour',
        target: '#videoTarget'
      },
      {
        title: 'Reviews',
        target: '#reviewTarget'
      },
      {
        title: 'Pricing',
        target: '#pricingTarget'
      },
      { title: 'GET IT FREE' }
    ]
  })
}
</script>

<style scoped>

.none__case:nth-child(n+1) > button {
  text-transform: none;
  font-family: NunitoSans;
  font-size: 15px;
}

.toolbar__items:nth-last-child(-2n+2) > button {
  background-color: white !important;
  border-radius: 6px;
  box-shadow: 0px 6px 12px 0 rgba(40, 43, 49, 0.08);
  color: black;
  width: 132px;
  height: 40px;
  font-size: 14px;
  font-weight: bold;
  font-family: NunitoSans;
}

.toolbar__title {
  color: white;
  font-family: NunitoSans;
  font-size: 20px;
  font-weight: 800;
}

.alg__img {
  display: flex;
  justify-content: flex-end;
  position: relative;
  height: 600px;
}

.alg__img > img {
  position: absolute;
}

#mainTitle {
  font-family: NunitoSans;
  font-size: 35px;
  color: white;
  text-align: left;
  padding: 44px 0;
}
#mainTitle > span {
  font-weight: 300;
}
.menu__hidden {
  position: absolute;
  left: 100%;
  height: 100vh;
}

.ovr__hd {
  overflow: hidden;
  position: relative;
}

.adaptive__space__between {
  margin-top: 50px;
}

.is-active {
  left: 0;
  height: 300px;
  display: flex;
  flex-flow: column;
  width: 100%;
  background-color: #ffffff;
  z-index: 55555;
  top: 0;
  justify-content: space-evenly;
  align-items: center;
}

.none__case > .btn__free {
  width: 132px;
  height: 40px;
  border-radius: 6px;
  background-color: #1f1d1d;
  display: flex;
  color: white;
  align-items: center;
  justify-content: center;
  box-shadow: 0px 6px 12px 0 rgba(40, 43, 49, 0.08);
}

@media (min-width: 960px) and (max-width: 1700px){
  .adaptive__space__between {
    justify-content: space-between;
  }
}
</style>
