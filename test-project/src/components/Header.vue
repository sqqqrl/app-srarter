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
          <v-list-tile>
            <a class="group__btn" href="#">Features</a>
            <a class="group__btn" href="#">Video Tour</a>
            <a class="group__btn" href="#">Reviews</a>
            <a class="group__btn" href="#">Pricing</a>
            <a class="group__btn" href="#">GET IT FREE</a>
          </v-list-tile>
        </v-list>
      </v-menu>
    <v-toolbar  flat dark class="hidden-sm-and-down ovr__hd">
      <v-toolbar-title>AppStarter</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="align-center none__case">
        <v-btn class="mr-3" flat>Features</v-btn>
        <v-btn class="mr-3" flat>Video Tour</v-btn>
        <v-btn class="mr-3" flat>Reviews</v-btn>
        <v-btn class="mr-3" flat>Pricing</v-btn>
        <v-btn class="white round mr-3">GET IT FREE</v-btn>
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
  data () {
    return {
      active: false
    }
  },
  methods: {
    click () {
      this.active = !this.active
    }
  }
}
</script>

<style scoped>
.round {
  border-radius: 6px;
  box-shadow: 0px 6px 12px 0 rgba(40, 43, 49, 0.08);
  color: black;
  width: 132px;
  height: 40px;
  font-size: 14px;
  font-weight: bold;
  font-family: NunitoSans;
}

.none__case > button:nth-child(n+1) {
  text-transform: none;
  font-family: NunitoSans;
  font-size: 15px;
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
