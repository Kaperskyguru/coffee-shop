<template>
  <v-row class="menu">
    <v-col
      :lg="12"
      :md="12"
      :align-self="right"
      justify-self="end"
    >
      <Menu />
    </v-col>
    <v-row>
      <v-col
        lg="6"
        md="6"
        sm="6"
      >
        <CoffeeText :title="title" class="mb-10" />
        <Button width="180" />
      </v-col>
      <v-col
        md="6"
        lg="6"
        :align-self="start"
        class="hidden-sm-and-down"
      >
        <v-img src="/coffeebeans.png" class="coffeeimg" />
      </v-col>
    </v-row>
  </v-row>
</template>

<script>
import Menu from '~/components/navigation/Menu'
import CoffeeText from '~/components/texts/CoffeeText'
import Button from '~/components/buttons/Button'
export default {
  components: {
    Menu,
    CoffeeText,
    Button
  },
  data () {
    return {
      title: 'A cup of coffee is one of the most important, simple pleasures in life.'
    }
  }
}
</script>

<style scoped>
.menu{
position: relative;
z-index: 1;
}

 .coffeeimg {
  max-width: 400px !important;
  /* max-height: 400px !important; */
   /* left: unset; */
   position: relative;
}

</style>
