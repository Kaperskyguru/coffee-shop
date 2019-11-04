<template>
  <div class="gallery">
    <v-col cols="12" sm="12" offset-sm="">
      <div class="mx-auto text-center">
        <h1 class="black--text">
          #NOANSACOFFEE
        </h1>
        <p>Coffee perfection since 1927</p>
      </div>
    </v-col>
    <v-row class="gallery">
      <v-col cols="12" sm="12" offset-sm="" class="gallery">
        <v-card flat>
          <v-container fluid class="gallery">
            <v-row>
              <v-col
                v-for="n in 12"
                :key="n"
                class="d-flex child-flex gallery"
                cols="2"
              >
                <v-card flat tile class="d-flex">
                  <v-img
                    :src="`https://picsum.photos/500/300?image=${n * 5 + 10}`"
                    :lazy-src="`https://picsum.photos/10/6?image=${n * 5 + 10}`"
                    aspect-ratio="1"
                    class="grey lighten-2"
                  >
                    <template v-slot:placeholder>
                      <v-row
                        class="fill-height ma-0"
                        align="center"
                        justify="center"
                      >
                        <v-progress-circular indeterminate color="grey lighten-5" />
                      </v-row>
                    </template>
                  </v-img>
                </v-card>
              </v-col>
            </v-row>
          </v-container>
        </v-card>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  components: {
  }
}
</script>

<style scoped>
  .gallery{
    margin: 0 !important;
    padding: 0 !important;
    border:0 !important;

  }

  p{
    font-size: 1rem;
  }

h1{
  font-weight: 700
}
</style>
