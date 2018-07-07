<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
@font-face{
  font-family: 'NunitoSans';
  src: url('./assets/fonts/NunitoSans-Regular.ttf');
}

.btn__download__watch {
  font-family: NunitoSans;
  font-size: 17px;
  font-weight: bold;
  letter-spacing: 0.9px;
  height: 50px;
  border-radius: 6px;
  text-transform: none;
}

.download {
  background-image: linear-gradient(135deg, #ff8e64, #ffe641);
  box-shadow: 0px 6px 12px 0 rgba(40, 43, 49, 0.08);
  color: white;
}

.bg__theme {
  background-image: url('./assets/img/bg1.png');
  background-size: cover;
  background-repeat: no-repeat;
  margin-bottom: 200px;
}

.list {
  display: flex;
  flex-flow: column;
  justify-content: space-around;
  align-items: center;
  height: 300px;
  background-color: #ffffff;
  padding: 15px 0;
}

.menu__content {
  width: 100%;
}

.menu__activator {
  position: absolute;
  right: 0;
}

.list__tile > a {
  font-family: NunitoSans;
  font-size: 15px;
  font-weight: normal;
  font-style: normal;
  font-stretch: normal;
  letter-spacing: normal;
  color: #333232;
  text-decoration: none;
}

</style>
