<template>
  <div class="bg-veryDarkBlue w-screen h-screen">
    <HeaderComponent />
    <TheMain />
  </div>
</template>

<script>
  import HeaderComponent from './components/layout/HeaderComponent.vue'
  import TheMain from './pages/TheMain.vue'

export default {
  name: 'App',
  components:{ HeaderComponent, TheMain },
}
</script>

<style>
</style>
