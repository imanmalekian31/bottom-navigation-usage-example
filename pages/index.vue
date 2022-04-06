<template>
  <div>
    <Tutorial />
    <GrowBottomNavigation v-model="selected" :options="options" />
  </div>
</template>

<script>
import { GrowBottomNavigation } from 'bottom-navigation-vue'

export default {
  components: { GrowBottomNavigation },
  data: () => ({
    selected: 1,
    options: [
      { id: 1, icon: 'fa-solid fa-home', title: 'Home', color: '#5639af' },
      { id: 2, icon: 'fa-solid fa-magnifying-glass', title: 'Search', color: '#ac4793' },
      { id: 3, icon: 'fa-solid fa-heart', title: 'Likes', color: '#e2a93a' },
      { id: 4, icon: 'fa-solid fa-gear', title: 'Settings', color: '#4493a7' }
    ]
  })
}
</script>
