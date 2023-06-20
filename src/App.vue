<script>
  import AppHeader from './components/AppHeader.vue';
  import AppMain from './components/AppMain.vue';
  import AppFooter from './components/AppFooter.vue';
  import AppNav from './components/AppNavContent.vue';
  export default {
    components:{
      AppHeader,
      AppMain,
      AppFooter,
      AppNav,
  }}

</script>

<template >
  <div>
    <AppHeader />
  </div>
  <div>
    <AppMain/>
  </div>
  <div>
    <AppNav />
  </div>
  <div>
    <AppFooter/>
  </div>
</template>


<style lang="scss">
  @use './styles/generals' as *
</style>