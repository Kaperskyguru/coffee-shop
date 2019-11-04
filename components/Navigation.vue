<template>
  <v-toolbar
    dense
    floating
    flat
    class="menu"
  >
    <v-toolbar-side-icon />
    <v-spacer />
    <v-toolbar-items class="menu-items">
      <v-btn text>
        SHOP
      </v-btn>
      <v-btn text>
        WHOLESALE
      </v-btn>
      <v-btn text>
        LOCATIONS
      </v-btn>
      <v-btn text>
        OUR STORY
      </v-btn>
    </v-toolbar-items>
    <v-btn icon>
      <v-icon>mdi-magnify</v-icon>
    </v-btn>
    <v-btn icon>
      <v-icon>mdi-heart</v-icon>
    </v-btn>
  </v-toolbar>
</template>

<script>
export default {
  name: 'Navigation'
}
</script>
<style scoped>
.menu-items button{
  font-weight: 400;
    font-size: .6rem;
    text-transform: uppercase;
}
.menu{
  display: inline;
  z-index: -1
}
</style>
