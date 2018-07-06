<template>
  <v-flex xs10 offset-xs1>
    <v-layout align-center column dark class="m150">
      <h1 class="ans">How <span>does it work</span></h1>
      <v-container fluid row wrap>
        <v-layout justify-center row wrap>
          <v-flex class="different__grd" xs12 sm7 md4 lg3>
            <div class="grd__div">
              <i class="fas fa-sync"></i>
            </div>
            <h2>Sync <span>across all devices</span></h2>
            <span>
              This sounded nonsense to Alice, so she said nothing, but set off at once toward the Red Queen. To her surprise.
            </span>
            <a href="#">Watch video</a>
          </v-flex>

          <v-flex class="different__grd ml-5 mr-5" xs12 sm7 md4 lg3>
            <div class="grd__div">
              <i class="fas fa-inbox"></i>
            </div>
            <h2>All emails <span>in one place</span></h2>
            <span>
              This sounded nonsense to Alice, so she said nothing, but set off at once toward the Red Queen. To her surprise.
            </span>
            <a href="#">Watch video</a>
          </v-flex>

          <v-flex class="different__grd" xs12 sm7 md4 lg3>
            <div class="grd__div">
              <i class="far fa-bell"></i>
            </div>
            <h2>Notifications <span>about sales</span></h2>
            <span>
              This sounded nonsense to Alice, so she said nothing, but set off at once toward the Red Queen. To her surprise.
            </span>
            <a href="#">Watch video</a>
          </v-flex>
        </v-layout>
      </v-container>
    </v-layout>
  </v-flex>
</template>

<script>
export default {
}
</script>

<style scoped>

.ans {
  font-family: NunitoSans;
  font-size: 35px;
  letter-spacing: 0.9px;
}

.ans > span {
  font-weight: 300;
}

.different__grd {
  width: 370px;
  height: 380px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  border-radius: 12px;
  background-color: #ffffff;
  box-shadow: 0px 1px 3px 0 rgba(32, 33, 39, 0.12);
  padding: 40px;
}

.different__grd > a {
  font-family: NunitoSans;
  font-size: 14px;
  color: #469af4;
  margin-top: 26px;
}

.different__grd:nth-child(1) > .grd__div {
  background-image: linear-gradient(135deg, #7956ec, #2fb9f8);
}
.different__grd:nth-child(2) > .grd__div {
  background-image: linear-gradient(135deg, #ff8e64, #ffe641);
}
.different__grd:nth-child(3) > .grd__div {
  background-image: linear-gradient(135deg, #ad2ab9, #ff618c);
}

.grd__div {
  width: 70px;
  height: 70px;
  border-radius: 6px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.grd__div > i {
  font-size: 24px;
  -webkit-text-fill-color: #ffffff !important;
}

.different__grd > h2 {
  margin: 30px 0 20px 0;
  font-family: NunitoSans;
  font-size: 20px;
  color: #282b31;
}

.different__grd > h2 > span {
  font-weight: 300;
}

.different__grd > span {
  font-family: NunitoSans;
  font-size: 14px;
  letter-spacing: normal;
  text-align: center;
  color: #676c75;
}

.m150 {
  margin: 150px 0;
}

@media (max-width: 959px){
  .different__grd:nth-child(2) {
    margin: 10px 0 !important;
  }
  .m150 {
    margin: 0 0;
  }
}

@media (min-width: 959px) and (max-width: 1260px){
  .different__grd:nth-child(n+1) {
    margin: 6px 6px !important;
  }
}
</style>
