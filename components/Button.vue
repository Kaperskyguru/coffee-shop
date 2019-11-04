<template>
  <div>
    <v-btn
      rounded
      :width="width"
      class="btn"
      large
      depressed
      color="yellow darken-1"
      light
    >
      <v-icon left>
        mdi-thumb-up
      </v-icon>
      {{ title }}
    </v-btn>
  </div>
</template>
<script>
export default {
  props: {
    title: {
      type: String,
      default: 'Shop Now'
    },
    width: {
      type: Number,
      default: undefined
    }

  }
}
</script>
<style scoped>
.btn{
    text-transform: capitalize;
}
</style>
