<template>
  <div class="tradingview-widget-container">
    <div class="tradingview-widget-container__widget"></div>
  </div>
</template>

<script>
export default {
  mounted() {
    const script = document.createElement('script')
    script.type = 'text/javascript'
    script.async = true
    script.src = 'https://s3.tradingview.com/external-embedding/embed-widget-ticker-tape.js'
    script.innerHTML = JSON.stringify({
      symbols: [
        {
          proName: 'BITSTAMP:BTCUSD',
          title: 'Bitcoin'
        },
        {
          description: 'Ethereum',
          proName: 'BINANCE:ETHUSDT'
        },
        {
          description: 'BNB',
          proName: 'BINANCE:BNBUSDT'
        },
        {
          description: 'XRP',
          proName: 'BINANCE:XRPUSDT'
        },
        {
          description: 'Cardano',
          proName: 'BITFINEX:ADAUSD'
        },
        {
          description: 'Litecoin',
          proName: 'BYBIT:LTCUSDT'
        }
      ],
      showSymbolLogo: true,
      colorTheme: 'light',
      isTransparent: false,
      displayMode: 'adaptive',
      locale: 'fr'
    })
    const container = document.querySelector('.tradingview-widget-container__widget')
    container.appendChild(script)
  }
}
</script>

<style>
.tradingview-widget-container {
  margin: 0 auto;
  max-width: 100%;
}
</style>