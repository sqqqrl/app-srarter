<template>
  <v-layout column class="bg__grey">
    <v-flex xs12 class="bg__theme mb-200px">
      <v-flex xs10 offset-xs1>
        <header>
          <page-header />
        </header>
      </v-flex>
    </v-flex>
    <v-flex class="main__content" xs12>
      <how-does-it-work />
      <logo />
      <tablet />
      <download />
      <chess-board />
      <play-video />
      <reviews />
      <plans />
      <stay-in-touch />
    </v-flex>
    <v-flex xs12>
      <page-footer />
    </v-flex>
  </v-layout>
</template>

<script>
import PageHeader from './Header.vue'
import HowDoesItWork from './HowDoesItWork.vue'
import Logo from './Logo.vue'
import Tablet from './Tablet.vue'
import Download from './Download.vue'
import ChessBoard from './ChessBoard.vue'
import PlayVideo from './PlayVideo.vue'
import Reviews from './Reviews.vue'
import Plans from './Plans.vue'
import StayInTouch from './StayInTouch.vue'
import PageFooter from './Footer.vue'

export default {
  components: {
    PageHeader,
    HowDoesItWork,
    Logo,
    Tablet,
    Download,
    ChessBoard,
    PlayVideo,
    Reviews,
    Plans,
    StayInTouch,
    PageFooter
  }
}
</script>

<style scoped>
header {
  padding-top: 60px;
}

.bg__grey {
  background-color: #f8f9fa;
  overflow: hidden;
  position: relative;
}
.mb-200px {
  margin-bottom: 200px;
}

@media (max-width: 1800px){
  .mb-200px {
    margin-bottom: 20px;
  }
}
</style>
