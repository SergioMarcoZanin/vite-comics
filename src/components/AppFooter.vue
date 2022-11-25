<script>
import AppLists from "../components/AppLists.vue";
import FooterFooter from "../components/FooterFooter.vue";
export default {
  name:"AppFooter",
  components: {
    AppLists,
    FooterFooter
  }
}
</script>

<template>
    <footer>
        <AppLists/>
        <FooterFooter/>
    </footer>
</template>

<style scoped lang="scss">
</style>