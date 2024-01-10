<template>
  <AppHeader />

  <AppMain />

  <TreatmentsList />

  <AppFooter />
</template>
  
  
<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import TreatmentsList from './components/TreatmentsList.vue';

export default {
  components: {
    AppHeader,
    AppMain,
    TreatmentsList,
    AppFooter
  }

}
</script>
  
  
  
<style lang="scss">
@use './styles/general.scss' as *;
</style>
