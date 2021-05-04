<template>
  <v-card rounded="xl">
    <v-card-title>Strength</v-card-title>
    <v-card-text>
    <iframe width="100%" height="400" src="https://s.tradingview.com/embed-widget/technical-analysis/?locale=en#%7B%22interval%22%3A%221m%22%2C%22width%22%3A425%2C%22isTransparent%22%3Afalse%2C%22height%22%3A450%2C%22symbol%22%3A%22BINANCE%3ABNBUSDT%22%2C%22showIntervalTabs%22%3Atrue%2C%22colorTheme%22%3A%22light%22%2C%22utm_source%22%3A%22www.tradingview.com%22%2C%22utm_medium%22%3A%22widget_new%22%2C%22utm_campaign%22%3A%22technical-analysis%22%7D" frameborder="0"></iframe>
    </v-card-text>
  </v-card>
</template>

<script>
export default {
  head() {
    return {
      script: [
        {
          src:
            'https://s3.tradingview.com/external-embedding/embed-widget-technical-analysis.js',
            
        },
      ],
    }
  },
  mounted() {
       
  },
}
</script>

<style>
</style>