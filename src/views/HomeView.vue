<template>
  <div class="home">
    <BannerPresa />
    <GroupCards />
  </div>
</template>

<script>
// @ is an alias to /src
import BannerPresa from '@/components/BannerPresa.vue'
import GroupCards from '@/components/GroupCards.vue'

export default {
  name: 'HomeView',
  components: {
    BannerPresa,
    GroupCards, 
  }
}
</script>
