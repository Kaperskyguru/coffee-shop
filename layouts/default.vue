<template>
  <v-app light fluid>
    <transition name="fade">
      <header id="header" class="brown lighten-5">
        <v-container>
          <Header />
        </v-container>
      </header>
    </transition>

    <transition name="fade">
      <v-content transition="slide-x-transition" class="white">
        <nuxt />
      </v-content>
    </transition>
    <v-container fluid class="white--text foot">
      <div class="text-center d-flex flex-column justify-center ma-10 pa-10">
        <h1 class="pa-2">
          Would you like to hear from us?
        </h1>
        <p>Submit your email address for our newsletter</p>
        <v-form class="mx-auto">
          <v-text-field
            v-model="email"
            required
            placeholder="yourname@mail.com"
            class="text-center"
          />
        </v-form>
      </div>
    </v-container>
    <v-footer class="black">
      <v-container>
        <span class="">All rights reserved &copy; 2019</span>
        <span class="float-right">+2348145655380</span>
        <div class="clearfix" />
      </v-container>
    </v-footer>
  </v-app>
</template>

<script>
import Header from '~/components/navigation/Nav.vue'
export default {
  components: {
    Header
  },
  data () {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire'
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js'
    }
  }
}
</script>
<style scoped>
  #header{
    height: 500px;
    background: #efebe9;
  }
  .foot{
    padding:0;
    background: #1B1B1B;
    color: #f5f5f5 !important;
  }

  .foot >>> input{
    text-align: center;
     width: 400px;
    color: #f5f5f5 !important;
  }

  .foot >>> input::placeholder{
    font-size: 1rem;
    color: rgb(128, 128, 128) !important;
  }

  .foot >>> .v-text-field__slot{
    width: 400px;
  }

  .foot >>> .v-input__slot{
    border-bottom: 2px solid white;
    color: #f5f5f5 !important;
  }

span{
  color: rgb(97, 97, 97) !important;
}

.fade-enter-active, .fade-leave-active {
  transition-property: opacity;
  transition-duration: .25s;
}

.fade-enter-active {
  transition-delay: .25s;
}

.fade-enter, .fade-leave-active {
  opacity: 0
}
</style>

<style lang="scss">

  html {
  font-size: 16px !important;
  @media screen and (min-width: 900px) {
    font-size: 10px !important;
  }
  @media screen and (min-width: 1200px) {
    font-size: 20px !important;
  }

}
  body{font-size: 16px;}
</style>
