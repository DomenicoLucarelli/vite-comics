<script>
import AppHeader from './components/AppHeader.vue'
import AppJumbo from './components/AppJumbo.vue'
import AppFrstSection from './components/AppFrstSection.vue'
import AppComics from './components/AppComics.vue'
import AppLinks from './components/AppLinks.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  data() {
    return {

    }
  },

  components: {
    AppHeader,
    AppJumbo,
    AppFrstSection,
    AppComics,
    AppLinks,
    AppFooter,
  }

}
</script>

<template>
  <AppHeader></AppHeader>
  <AppJumbo></AppJumbo>
  <AppFrstSection></AppFrstSection>
  <AppComics></AppComics>
  <AppLinks></AppLinks>
  <AppFooter></AppFooter>
</template>

<style lang="scss">
.container {
  width: 1000px;
  margin: auto;
}
</style>