<template>
  <div>
    <nuxt />
    <CurvedBottomNavigation v-model="selected" :options="options" replace-route />
  </div>
</template>

<script>
import { CurvedBottomNavigation } from 'bottom-navigation-vue'

export default {
  components: { CurvedBottomNavigation },
  data: () => ({
    selected: 1,
    options: [
      {
        id: 1,
        icon: 'fa-solid fa-home',
        title: 'Home',
        color: '#5639af',
        path: { name: 'home' }
      },
      {
        id: 2,
        icon: 'fa-solid fa-magnifying-glass',
        title: 'Search',
        color: '#ac4793',
        path: { name: 'search' }
      },
      {
        id: 3,
        icon: 'fa-solid fa-heart',
        title: 'Likes',
        color: '#e2a93a',
        path: { name: 'likes' }
      },
      {
        id: 4,
        icon: 'fa-solid fa-gear',
        title: 'Settings',
        color: '#4493a7',
        path: { name: 'settings' }
      }
    ]
  })
}
</script>
