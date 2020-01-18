<template>
      <div>
        <h2>Histórico de preços - Compra</h2><br>
        <div id="first">
          <h2>Data:   {{previousCurrency.yesterday.DATE}}</h2><br>
          <p><label>1 BTC:R$ </label> {{(previousCurrency.yesterday.BTC * 1.08).toFixed(2)}}</p><br><br>
          <p><label>1 ETH: R$ </label> {{previousCurrency.yesterday.ETH}}</p><br><br>
          <p><label>1 LTC: R$ </label> {{previousCurrency.yesterday.LTC}}</p>
        </div>
        <div id="second">
          <h2>Data:   {{previousCurrency.twoDays.DATE}}</h2><br>
          <p><label>1 BTC: R$ </label> {{(previousCurrency.twoDays.BTC * 1.08).toFixed(2)}}</p><br><br>
          <p><label>1 ETH: R$ </label> {{previousCurrency.twoDays.ETH}}</p><br><br>
          <p><label>1 LTC: R$ </label> {{previousCurrency.twoDays.LTC}}</p>
        </div>
        <div id="third">
          <h2>Data:   {{previousCurrency.threeDays.DATE}}</h2><br>
          <p><label>1 BTC: R$ </label> {{(previousCurrency.threeDays.BTC * 1.08).toFixed(2)}}</p><br><br>
          <p><label>1 ETH: R$ </label> {{previousCurrency.threeDays.ETH}}</p><br><br>
          <p><label>1 LTC: R$ </label> {{previousCurrency.threeDays.LTC}}</p>
        </div>
        <br>
        <h2>Histórico de preços - Venda</h2><br>
        <div id="first">
          <h2>Data:   {{previousCurrency.yesterday.DATE}}</h2><br>
          <p><label>1 BTC: R$ </label> {{(previousCurrency.yesterday.BTC / 1.08).toFixed(2)}}</p><br><br>
          <p><label>1 ETH: R$ </label> {{previousCurrency.yesterday.ETH}}</p><br><br>
          <p><label>1 LTC: R$ </label> {{previousCurrency.yesterday.LTC}}</p>
        </div>
        <div id="second">
          <h2>Data:   {{previousCurrency.twoDays.DATE}}</h2><br>
          <p><label>1 BTC: R$ </label> {{(previousCurrency.twoDays.BTC / 1.08).toFixed(2)}}</p><br><br>
          <p><label>1 ETH: R$ </label> {{previousCurrency.twoDays.ETH}}</p><br><br>
          <p><label>1 LTC: R$ </label> {{previousCurrency.twoDays.LTC}}</p>
        </div>
        <div id="third">
          <h2>Data:   {{previousCurrency.threeDays.DATE}}</h2><br>
          <p><label>1 BTC: R$ </label> {{(previousCurrency.threeDays.BTC / 1.08).toFixed(2)}}</p><br><br>
          <p><label>1 ETH: R$ </label> {{previousCurrency.threeDays.ETH}}</p><br><br>
          <p><label>1 LTC: R$ </label> {{previousCurrency.threeDays.LTC}}</p>
        </div>
        
      </div>
    </template>

    <script>
    export default {
      name: 'app',
      props: {
        previousCurrency: { type: Object }
      },
      data () {
        return {}
      }
    }
    </script>

     <style scoped>
    #first, #second, #third, #fourth, #fifth {
      border: 1px solid #F5CE00;
      padding: 2em 0em;
      max-width: 90%;
      margin: 3px auto;
    }
    #first p, #second p, #third p, #fourth p, #fifth p {
      display: inline-block;
      padding: 0em 1.5em;
      font-size: 1.0rem;
    }
    h2 { font-size: 1.0em; }
    </style>