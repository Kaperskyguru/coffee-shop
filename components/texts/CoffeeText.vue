
<template>
  <div class="coffeetext">
    <h5>Premium Coffee</h5>
    <p class="title">
      {{ title }} <!-- Quality coffee cultivated by Good -->
    </p>
    <p class="content">
      {{ content }}
    </p>
  </div>
</template>

<script>

export default {
  components: {
  },

  props: {
    title: {
      type: String,
      default: 'Quality coffee cultivated by Good'
    },
    content: {
      type: String,
      default: ''
    }

  }

}

</script>

<style scoped>
h5{
    font-size: .6rem;
    font-weight: 400;
    text-transform: uppercase;
}

.coffeetext .title{
    font-weight: 300;
    font-size: 1.9rem !important;
    text-align: left;
}

.coffeetext .content{
    font-size: .7rem;
}

div{
    width: 500px;
    height: 140px;
}
</style>
