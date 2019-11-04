<template>
  <v-row v-if="switchValue">
    <v-col
      md="6"
    >
      <CoffeeText :content="desc" />
      <Button class="bt" />
    </v-col>

    <v-col
      md="6"
    >
      <CoffeeImageCard :curve="curve" />
    </v-col>
  </v-row>
  <v-row v-else>
    <v-col
      md="6"
    >
      <CoffeeImageCard :curve="curve" />
    </v-col>

    <v-col
      md="6"
    >
      <CoffeeText :content="desc" />
      <Button class="bt" />
    </v-col>
  </v-row>
</template>

<script>
import CoffeeImageCard from '~/components/coffeeinfo/CoffeeImageCard'
import CoffeeText from '~/components/texts/CoffeeText'
import Button from '~/components/buttons/Button'
export default {
  components: {
    CoffeeImageCard,
    CoffeeText,
    Button
  },
  props: {
    curve: {
      type: String,
      default: 'left'
    },
    switch: {
      type: Boolean,
      default: false
    }
  },
  data () {
    return {
      desc: 'Our love for specialty coffee is never-ending. With over 365 days a year at origin working with the best growers on the planet, only the best beans make the grade',
      switchValue: this.switch
    }
  }

}
</script>

<style scoped>
.bt{
    margin-top: 40px;
}
</style>
