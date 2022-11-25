<script>
import AppShops from '../components/AppShops.vue';
import AppContent from '../components/AppContent.vue';
export default {
  name:"AppMain",
  components: {
    AppShops,
    AppContent
  }
}
</script>

<template>
    <main>
        <AppContent/>
        <AppShops/>
    </main>
</template>

<style scoped lang="scss">
main{
    background-color: black;
    color: white;
}
</style>