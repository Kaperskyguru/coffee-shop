<template>
  <v-row class="menu">
    <v-col
      :lg="3"
      :md="3"
      align-self="left"
    >
      <Logo />
    </v-col>
    <v-col
      :lg="9"
      :md="9"
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
        <CoffeeText :title="title" />
        <Button width="180" />
      </v-col>
      <v-col
        md="6"
        lg="6"
        :align-self="start"
      >
        <v-img src="/coffeebeans.png" class="coffeeimg" />
      </v-col>
    </v-row>
  </v-row>
</template>

<script>
import Menu from '~/components/Navigation'
import Logo from '~/components/Logo'
import CoffeeText from '~/components/CoffeeText'
import Button from '~/components/Button.vue'
export default {
  components: {
    Menu,
    Logo,
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
