<template>
  <v-row>
    <v-col
      v-for="(service, i) in services"
      :key="i"
      md="3"
    >
      <Service :design="service.design" :content="service.content" :icon="service.icon" />
    </v-col>
  </v-row>
</template>

<script>
import Service from '~/components/services/Service'
export default {
  components: {
    Service
  },
  data () {
    return {
      services: [
        { content: 'Quality coffee cultivated by Good', icon: 'mdi-magnify', design: true },
        { content: 'Flavour single origin froth in spoon iced', icon: 'mdi-watch', design: false },
        { content: 'Milk grounds chicory beans single origin', icon: 'mdi-tilde', design: false },
        { content: 'Coffee irish robusta spoon robust', icon: 'mdi-tennis', design: false }
      ]
    }
  }

}
</script>

<style>

</style>
