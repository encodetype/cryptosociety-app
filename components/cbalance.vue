<template>
  <v-card elevation="2" outlined rounded="xl">
          <v-card-text>
            <center>
              <v-img
                :src="img"
                width="80"
                absolute

                
                class="mt-n11 rounded-circle"
              ></v-img>
              <span class="display-1 text--primary font-weight-black"
                >{{amount}}</span
              >
              <p class="subtitle-1">{{dest}}</p>
            </center>
          </v-card-text>
        </v-card>
</template>

<script>
export default {
    props:{
        img:String,
        amount:String,
        dest:String
    }
}
</script>

<style>

</style>