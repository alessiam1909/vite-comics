<script>
import AppHeader from './components/AppHeader.vue'
import AppBody from './components/AppBody.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  components: {
    AppHeader,
    AppBody,
    AppFooter
  }
}
</script>

<template>
  <AppHeader />
  <AppBody />
  <AppFooter />
</template>

<style lang="scss">
@use './src/styles/generals.scss' as *;
</style>
