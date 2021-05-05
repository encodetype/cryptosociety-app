<template>
  <div>
    <v-row>
      <v-col cols="12" md="12">
        <h2 class="display-1 font-weight-black">Dashbord</h2>
      </v-col>
    </v-row>
    <v-row>
      <v-col cols="12" md="3">
        <cbalance
          img="https://icons.iconarchive.com/icons/cjdowner/cryptocurrency-flat/1024/Ethereum-ETH-icon.png"
          amount="1,000 ETH"
          dest="Amount of ETH"
        ></cbalance>
      </v-col>
      <v-col cols="12" md="3">
        <cbalance
          img="https://bitcoin.org/img/icons/opengraph.png?1619021447"
          amount="1.5 BTC"
          dest="Amount of BTC"
        ></cbalance>
      </v-col>
      <v-col cols="12" md="3">
        <cbalance
          img="https://upload.wikimedia.org/wikipedia/commons/a/a1/Wallet_App_icon_iOS_12.png"
          amount="$12,840"
          dest="Amount of USD"
        ></cbalance>
      </v-col>
      <v-col cols="12" md="3">
        <cbalance
          img="https://avatars.githubusercontent.com/u/9450785?v=4"
          amount="500 CRS"
          dest="CRS Coin"
        ></cbalance>
      </v-col>
    </v-row>

    <v-row>
      <v-col cols="12" md="9">
        <minchart></minchart>
      </v-col>
      <v-col cols="12" md="3">
        <strength></strength>
      </v-col>
    </v-row>

    <v-row>
      <v-col cols="12" md="3">
          <historyPar type="Sell Order"></historyPar>
      </v-col>
       <v-col cols="12" md="3">
          <historyPar type="Buy Order"></historyPar>
      </v-col>
        <v-col cols="12" md="3">
            <swap></swap>
        </v-col>
     </v-row>

  </div>
</template>

<script>
import cbalance from '@/components/cbalance'
import minchart from '@/components/minchart'
import strength from '@/components/strength'
import historyPar from "@/components/pairhistory"
import swap from "@/components/swap"
export default {
  components: {
    cbalance,
    minchart,
    strength,historyPar,swap
  },
}
</script>

<style>
</style>