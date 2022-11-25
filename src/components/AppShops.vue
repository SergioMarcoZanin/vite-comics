<script>
export default {
  name:"AppShops",
  data(){
    return {
        shops:[
          {
            title:"DIGITAL COMICS",
            img:"src/assets/buy-comics-digital-comics.png"
          },
          {
            title:"DC MERCHANDISE",
            img:"src/assets/buy-comics-merchandise.png"
          },
          {
            title:"SUBSCRIPTION",
            img:"src/assets/buy-comics-subscriptions.png"
          },
          {
            title:"COMIC SHOP LOCATOR",
            img:"src/assets/buy-comics-shop-locator.png"
          },
          {
            title:"DC POWER VISA",
            img:"src/assets/buy-dc-power-visa.svg"
          }   
        ],
    }
  }
}
</script>

<template>
    <section class="shops">
        <div class="container">
            <div class="shop" v-for="shop in shops">
                <img :src="shop.img" :alt="shop.title">
                <span>{{shop.title}}</span>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
    .shops{
        background-color: var(--primary-color);
        color: white;
        font-weight: bold;
        .shop{
            display: flex;
            align-items: center;
            padding: 3.125rem .625rem;
            img{
                max-width: 3.125rem;
                max-height: 3.125rem;
                margin-right: 1rem;
            }
        }
    }
</style>