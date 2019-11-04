<template>
  <div :class="{ wrapper:designed }" class="wrapper1">
    <div :class="{ curve:designed }">
      <v-icon large class="ico">
        {{ icon }}
      </v-icon>
    </div>
    <div class="content-wrapper">
      <p class="content">
        {{ content }}
      </p>
    </div>
  </div>
</template>

<script>
export default {

  props: {
    icon: {
      type: String,
      default: 'mdi-magnify'
    },
    content: {
      type: String,
      default: 'Quality coffee cultivated by Good'
    },
    design: {
      type: Boolean,
      default: false
    }
  },

  data () {
    return {
      designed: this.design
    }
  }

}
</script>

<style scoped>
.wrapper{
    border-top-right-radius: 30px;
    background: #ffe5b4;
}
.wrapper1{
    max-width: 130px;
    max-height: 200px;
}
.ico{
    margin-top: 30px;
    margin-left:20px;
    margin-bottom: 20px;
}
p.content{
    margin-left:5px;
    font-size: .9rem;
    font-weight: 500;
    padding-bottom: 20px !important;
}

.curve{
    background:orange;
    width: 130px;
    height: 70px;
    border-radius: 0 90px 200px 100%/50px;
}
.content-wrapper{
    padding: 10px 10px 0px 10px;
}
</style>
