<template>
  <v-img
    :src="`https://picsum.photos/500/300?image=${n * 5 + 10}`"
    :lazy-src="`https://picsum.photos/10/6?image=${n * 5 + 10}`"
    aspect-ratio="1"
    class="grey lighten-2"
  >
    <v-card flat tile class="d-flex">
      <template v-slot:placeholder>
        <v-row
          class="fill-height ma-0"
          align="center"
          justify="center"
        >
          <v-progress-circular indeterminate color="grey lighten-5" />
        </v-row>
      </template>
    </v-card>
  </v-img>
</template>

<script>
export default {
  props: {
    n: {
      type: Number,
      default: 1
    }
  }

}
</script>

<style scoped>

</style>
