<template>
  <v-card rounded="xl" >
    <v-card-title> BNB (Binance smart chain) </v-card-title>
    <v-card-text>
    <div class="tradingview-widget-container">
  <div id="tradingview_33aa4"></div>
    </div>
    </v-card-text>
  </v-card>
</template>

<script>
export default {
  head() {
    return {
      script: [{ src: 'https://s3.tradingview.com/tv.js' }],
    }
  },
  mounted() {
    new TradingView.widget({
      width: '100%',
      height: 400,
      symbol: 'BNB/USDT',
      interval: 'D',
      timezone: 'Etc/UTC',
      theme: 'light',
      style: '1',
      locale: 'en',
      toolbar_bg: '#f1f3f6',
      enable_publishing: false,
      allow_symbol_change: true,
      container_id: 'tradingview_33aa4',
    })
  },
}
</script>

<style>
</style>