<template>
  <div>
    <div class="text-center box mx-auto" style="">
      <p class="first">
        BUY NOW
      </p>
      <h2>Our Best Deals</h2>
      <p class="content">
        Coffee company with a straightforward mission; to make an office and on-the-go cup of coffee that we've like to drink ourselves
      </p>
    </div>

    <v-row>
      <v-col
        md="4"
      >
        <Card />
      </v-col>

      <v-col
        md="4"
      >
        <Card />
      </v-col>

      <v-col
        md="4"
      >
        <Card />
      </v-col>
    </v-row>
  </div>
</template>

<script>
import Card from '~/components/BestDealCard'
export default {
  components: {
    Card
  }
}
</script>

<style scoped>
.box{
    margin-top: 50px;
    margin-bottom: 30px;
    width: 520px;
}

.box p.first{
    font-size: .6rem;
    text-transform: uppercase;
    font-weight: 300
}

.box h2{
    font-size: 2rem;
    font-weight: 400;
}

.box p.content {
font-weight: 300
}
</style>
