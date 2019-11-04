<template>
  <v-layout
    column
    justify-center
    align-center
  >
    <v-container class="mt-10 mb-10">
      <Services />
    </v-container>

    <v-container class="mt-10 mb-10">
      <CoffeeInfo curve="right" />
    </v-container>

    <v-container fluid class="mt-10 pa-10" style="background:rgba(255,255,224, 0.4)">
      <BestDeals />
    </v-container>

    <v-container class="mt-10 mb-10">
      <CoffeeInfo curve="left" switch="true" />
    </v-container>

    <v-container fluid class="gallery">
      <Gallery />
    </v-container>
  </v-layout>
</template>

<script>
import Services from '~/components/services/Services.vue'
import CoffeeInfo from '~/components/coffeeinfo/CoffeeInfo'
import BestDeals from '~/components/deals/BestDeal'
import Gallery from '~/components/Gallery/Gallery'
export default {
  components: {
    Services,
    CoffeeInfo,
    BestDeals,
    Gallery
  },
  data () {
    return {
      coffeetext: 'Our love for specialty coffee is never-ending. With over 365 days a year at origin working with the best growers on the planet, only the best beans make the grade'
    }
  }
}
</script>

<style  scoped>
  .gallery{
    margin: 0px !important;
    padding-top: 0px;
    border:0 !important;
  }
</style>
