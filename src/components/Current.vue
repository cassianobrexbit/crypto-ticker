<template>
      <div>
        <h2>Compra</h2><br>
        <div id="btc" class="currency">
          <label>1 BTC</label>
          <p>R${{(currentCurrency.BTC * 1.08).toFixed(2)}}</p>
        </div>
        <br><br>
        <div id="eth" class="currency">
          <label>1 ETH</label>
          <p>R${{(currentCurrency.ETH * 1.08).toFixed(2)}}</p>
        </div>
        <br><br>
        <div id="ltc" class="currency">
          <label>1 LTC</label>
          <p>R${{(currentCurrency.LTC * 1.08).toFixed(2)}}</p>
        </div>
        <br><br>
        <h2>Venda</h2><br>
        <div id="btc" class="currency">
          <label>1 BTC</label>
          <p>R${{(currentCurrency.BTC / 1.08).toFixed(2)}}</p>
        </div>
        <br><br>
        <div id="eth" class="currency">
          <label>1 ETH</label>
          <p>R${{(currentCurrency.ETH / 1.08).toFixed(2)}}</p>
        </div>
        <br><br>
        <div id="ltc" class="currency">
          <label>1 LTC</label>
          <p>R${{(currentCurrency.LTC / 1.08).toFixed(2)}}</p>
        </div>
      </div> 
    </template>
    
    <script>
    export default {
      name: 'app',
      props: {
        currentCurrency: { type: Object }
      }, 
      data () {
        return {}
      }
    }
    </script>

    <style scoped>
    .currency {
      border: 1px solid #F5CE00;
      border-radius: 15px;
      padding: 2em 0em;
      display: inline-block;
      width: 30%;
    }
    div p { font-size: 1.5rem; }
    h2 { font-size: 1.0em; }
    </style>