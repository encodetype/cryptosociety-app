<template>
  <v-card rounded="xl">
    <v-card-title>
      {{ type }}
    </v-card-title>

    <v-card-text>
        <v-card rounded="xl">
            <v-list  color="#F4F4F4">
                <v-list-item>
                     <img src="https://s3.cointelegraph.com/storage/uploads/view/bf7541e09a456a3fc6113ec9c7cdf408.png" width="60"/>
                     <v-spacer></v-spacer>
                     <h2 class="title">Get Litecoin</h2>
                       <v-spacer></v-spacer>
                       <v-btn icon>
                           <v-icon>mdi-animation-outline</v-icon>
                       </v-btn>
                </v-list-item>
            </v-list>
               
        </v-card>
    </v-card-text>

    <v-list class="mt-n6" background-color="#E4F2FD">
      <v-list-item>
        <span class="text--secondary">PRICE</span>
        <v-spacer></v-spacer>
        <span class="text--secondary">AMOUNT</span>
        <v-spacer></v-spacer>
        <span class="text--secondary">TOTAL</span>
      </v-list-item>

      <v-list-item link v-for="(p, i) in price" :key="i">
        <span class="text--primary font-weight-black">{{ p.p }}</span>
        <v-spacer></v-spacer>
        <span class="text--primary font-weight-black">{{ p.a }}</span>
        <v-spacer></v-spacer>
        <span class="text--primary font-weight-black"> $ {{ p.t }}</span>
      </v-list-item>
    </v-list>
  </v-card>
</template>

<script>
export default {
  props: {
    type: String,
  },
  data() {
    return {
      price: [
        {
          p: 82.3,
          a: 0.15,
          t: 1234.4,
        },
        {
          p: 82.3,
          a: 0.15,
          t: 1234.4,
        },
        {
          p: 82.3,
          a: 0.15,
          t: 1234.4,
        },
        {
          p: 82.3,
          a: 0.15,
          t: 1234.4,
        },
        {
          p: 82.3,
          a: 0.15,
          t: 1234.4,
        },
        {
          p: 82.3,
          a: 0.15,
          t: 1234.4,
        },
        {
          p: 82.3,
          a: 0.15,
          t: 1234.4,
        },
        {
          p: 82.3,
          a: 0.15,
          t: 1234.4,
        },
        {
          p: 82.3,
          a: 0.15,
          t: 1234.4,
        },
      ],
    }
  },
}
</script>

<style>
</style>