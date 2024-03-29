<template>
  <AppHeader />

  <AppMain />

  <TreatmentsList />

  <UpperFooter />

  <AppFooter />
</template>
  
  
<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import TreatmentsList from './components/TreatmentsList.vue';
import UpperFooter from './components/UpperFooter.vue';
import AppFooter from './components/AppFooter.vue'



export default {
  components: {
    AppHeader,
    AppMain,
    TreatmentsList,
    UpperFooter,
    AppFooter
  }

}
</script>
  
  
  
<style lang="scss">
@use './styles/general.scss' as *;
</style>
