<script>
    import AppTitle from './components/AppTitle.vue';
    import AppHero from './components/AppHero.vue';

    export default {
      name: 'App',
      components: {
        AppTitle,
        AppHero
      }
    }
</script>

<template>
  <div id="title">
    <AppTitle/>
    <AppHero/>
  </div>
</template>

<style scoped>
#title {
  margin-top: 2rem;
}
</style>
