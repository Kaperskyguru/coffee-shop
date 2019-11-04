<template>
  <div class="text-center">
    <v-card
      class="mx-auto"
      max-width="250"
      flat
      color="transparent"
    >
      <v-img
        src="https://cdn.vuetifyjs.com/images/cards/sunshine.jpg"
        height="250"
        max-width="200"
        class="mx-auto"
      />
      <v-card-title style="justify-content:center">
        <h4>
          Platinum
        </h4>
        <h2>Noansa Platinum Blend</h2>
        <Button title="$30.00" />
      </v-card-title>
    </v-card>
  </div>
</template>
<script>
import Button from '~/components/buttons/Button'
export default {
  components: {
    Button
  }
}
</script>
<style scoped>
h4{
font-size: .8rem;
font-weight: 300;
}
h2{
    text-align: center !important;
    font-size: 1rem;
    font-weight: 400
}

</style>
