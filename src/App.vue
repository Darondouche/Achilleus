<template>
  <BitcoinTicker />
  <NavBar />
  <router-view />
</template>

<script>
import NavBar from '@/components/NavBar.vue'
import BitcoinTicker from '@/components/BitcoinTicker.vue'

export default {
  name: 'App',
  components: {
    BitcoinTicker,
    NavBar
  }
}
</script>