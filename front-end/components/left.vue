<template>
  <v-navigation-drawer app floating >
    <v-list>
      <v-list-item>
        <v-list-item-avatar>
          <v-img
            src="https://avatars.githubusercontent.com/u/9450785?v=4"
            width="50"
          ></v-img>
        </v-list-item-avatar>
        <v-list-item-title>
          <span class="font-weight-black title"> Crypto Society </span>
        </v-list-item-title>
      </v-list-item>

      <div>
        <div class="text-center">
          <img
            src="https://cdn.vuetifyjs.com/images/john.jpg"
            alt="John"
            class="rounded-circle"
            width="80"
          />

          <h2 class="title">Hello ,Marquest</h2>
          <h2 class="subtitle-1 text--secondary mt-n2">Master Owner</h2>
        </div>
      </div>

      <div class="mt-8">
        <v-list-item link v-for="x in menu" :key="x.text">
          <v-list-item-icon>
            <v-img :src="x.img" width="25"></v-img>
          </v-list-item-icon>
          <v-list-item-title>
            <span class="font-weight-bold">{{ x.text }}</span>
          </v-list-item-title>
        </v-list-item>
      </div>
    </v-list>
  </v-navigation-drawer>
</template>

<script>
export default {
  data() {
    return {
      menu: [
        {
          url: '',
          text: 'Dashbord',
          img: '/icon/dashbord.svg',
        },
        {
          url: '',
          text: 'Dapp',
          img: '/icon/app.svg',
        },
        {
          url: '',
          text: 'Chart',
          img: '/icon/chart.svg',
        },
         {
          url: '',
          text: 'Master',
          img: '/icon/master.svg',
        },
         {
          url: '',
          text: 'Farm',
          img: '/icon/farm.svg',
        },
          {
          url: '',
          text: 'Swap',
          img: '/icon/swap.svg',
        },
      ],
    }
  },
}
</script>

<style>
</style>