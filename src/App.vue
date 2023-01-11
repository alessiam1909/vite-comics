<script>
import AppHeader from './components/AppHeader.vue'
import AppBody from './components/AppBody.vue'
import AppInfo from './components/AppInfo.vue'
import AppFooter from './components/AppFooter.vue'


export default {
  components: {
    AppHeader,
    AppBody,
    AppInfo,
    AppFooter
  }
}
</script>

<template>
  <AppHeader />
  <AppBody />
  <AppInfo/>
  <AppFooter />
</template>

<style lang="scss">
@use './src/styles/generals.scss' as *;
</style>
