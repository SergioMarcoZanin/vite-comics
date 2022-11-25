<script>
export default {
  name:"AppHeader",
  data() {
    return {
      links:[
        "CHARACTERS",
        "COMICS",
        "MOVIES",
        "TV",
        "GAMES",
        "COLLECTIBLES",
        "VIDEOS",
        "FANS",
        "NEWS",
        "SHOP"
      ]
    }
  }
}
</script>

<template>
  <header>
    <div class="container">
      <img src="../assets/dc-logo.png" alt="Logo DC">
      <ul>
        <li v-for="link in links"><a href="#">{{link}}</a></li>
      </ul>
    </div>
  </header>
</template>

<style scoped lang="scss">
img{
  padding: 1rem;
}
ul{
  display: flex;
  list-style: none;
  a{
    text-decoration: none;
    display: inline-block;
    padding:1.25rem ;
    color: black;
  }
}
</style>

