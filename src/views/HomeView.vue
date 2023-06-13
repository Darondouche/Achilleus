<template>
  <div class="home dark:bg-gray-800 dark:text-gray-100">
    <AchilleusPresa />
    <ConceptionAchilleus />
    <SpotInvestPresa />
    <BoostPresa />
    <GroupCards />
  </div>
</template>

<script>
// @ is an alias to /src
import AchilleusPresa from '@/components/AchilleusPresa.vue'
import GroupCards from '@/components/GroupCards.vue'
import SpotInvestPresa from '@/components/SpotInvestPresa.vue'
import BoostPresa from '@/components/BoostPresa.vue'
import ConceptionAchilleus from '@/components/ConceptionAchilleus.vue'

export default {
  name: 'HomeView',
  components: {
    AchilleusPresa,
    ConceptionAchilleus,
    SpotInvestPresa,
    BoostPresa,
    GroupCards, 
  }
}
</script>
