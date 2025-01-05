<template>
  <AppHeader />
  <AppStack id="stack" />
  <AppPortfolio />
  <AppAboutme />
  <AppContact id="section4" />
</template>

<script>
import AppHeader from './components/AppHeader.vue'
import AppStack from './components/AppStack.vue'
import AppPortfolio from './components/AppPortfolio.vue'
import AppAboutme from './components/AppAboutme.vue'
import AppContact from './components/AppContact.vue'
export default {
  components: { AppHeader, AppStack, AppPortfolio, AppAboutme, AppContact },
}
</script>

<style scoped></style>
