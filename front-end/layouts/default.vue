<template>
  <v-app   >
    <navi></navi>
    <left></left>
    <v-main class="bg" >
      <v-container  class="mx-4 mt-5"> 
          <nuxt></nuxt>
      </v-container>
      
    </v-main>
  </v-app>
</template>

<script>
import navi from '@/components/navi'
import left from '@/components/left'
export default {
  components: {
    navi,left
  },
}
</script>

<style>
.bg{
    background:#F9F9F9  !important;
}
</style>