
<template>
  <div>
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
    font-size: .7rem;
    font-weight: 400;
    text-transform: uppercase;
}

.title{
    text-transform: capitalize;
    font-weight: 300;
    font-size: 2.1rem !important;
    text-align: left;
}

.content{
    font-size: .95rem;
}

div{
    width: 500px;
    height: 140px;
}
</style>
