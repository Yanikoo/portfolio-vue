<template>
  <AppHeader />
  <AppStack />
  <AppPortfolio />
</template>

<script>
import AppHeader from './components/AppHeader.vue'
import AppStack from './components/AppStack.vue'
import AppPortfolio from './components/AppPortfolio.vue'
export default {
  components: { AppHeader, AppStack, AppPortfolio },
}
</script>

<style scoped></style>
