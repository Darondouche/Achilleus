<template>
  <div class="home dark:bg-gray-800 dark:text-gray-100">
    <AchilleusPresa />
    <ConceptionAchilleus />
    <LimitsAchilleus />
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
import LimitsAchilleus from '@/components/LimitsAchilleus.vue'

export default {
  name: 'HomeView',
  components: {
    AchilleusPresa,
    ConceptionAchilleus,
    LimitsAchilleus,
    SpotInvestPresa,
    BoostPresa,
    GroupCards, 
  }
}
</script>
