<template>
  <v-card   rounded="xl"     >
      <v-card-title>Swap Exchange</v-card-title>
      <v-card-subtitle>Exchange coin</v-card-subtitle>
      <v-card-text>
           <v-text-field
             
            label="From"
            outlined
            clearable
            class="rounded-xl"
          ></v-text-field>

            <v-text-field
             
            label="To"
             outlined
             clearable
             class="rounded-xl"
          ></v-text-field>

<v-btn large color="#00AAF0" dark  class="rounded-xl"  elevation="0" block>
             Exchange  Swap
          </v-btn>

      </v-card-text>
      <v-card-actions>
          
      </v-card-actions>
  </v-card>
</template>

<script>
export default {

}
</script>

<style>

</style>