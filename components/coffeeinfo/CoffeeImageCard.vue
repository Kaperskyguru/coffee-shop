<template>
  <div :class="[ curveType ? 'curve': 'curve-2'] " class="wrapper">
    <v-img :class="[ curveType ? 'curve': 'curve-2'] " src="https://picsum.photos/510/300?random" />
  </div>
</template>

<script>
export default {
  props: {
    curve: {
      type: String,
      default: 'left'
    }
  },

  data () {
    return {
      curveType: this.curve === 'right'
    }
  }
}
</script>

<style scoped>
.wrapper{
    max-width: 500px;
    max-height: 500px;
}

.curve{
    border-radius: 300px 300px 0px 300px;
}

.curve-2{
    border-radius: 300px 300px 300px 0px;
}
</style>
