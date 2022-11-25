<script>
export default {
  name:"AppLists",
  data() {
    return {
        links:[
        "Characters",
        "Comics",
        "Movies",
        "Tv",
        "Games",
        "Collectibles",
        "Videos",
        ],
        dc:[
            "Terms Of Use",
            "Privacy policy (new)",
            "Ad Choices",
            "Advertising",
            "Jobs",
            "Subscriptions",
            "Talent Workshop",
            "CPSC Certificaters",
            "Ratings",
            "Shop Help",
            "Contact Us"
        ],
        sites:[
            "DC",
            "MAD Magazine",
            "DC Kids",
            "DC universe",
            "DC Power Visa"
        ]
    }
  }
}
</script>

<template>
    <section class="footer-links">
        <div class="container">
            <div class="lists">
                <div>
                    <h3>DC COMICS</h3>
                    <ul>
                        <li v-for="link in links"><a href="#">{{link}}</a></li>
                    </ul>
                    <h3>SHOP</h3>
                    <ul>
                        <li><a href="#">Shop DC</a></li>
                        <li><a href="#">Shop DC Collectibles</a></li>
                    </ul>
                </div>
                <div>
                    <h3>DC</h3>
                    <ul>
                        <li v-for="elm in dc"><a href="#">{{elm}}</a></li>
                    </ul>
                </div>
                <div>
                    <h3>DC COMICS</h3>
                    <ul>
                        <li v-for="site in sites"><a href="#">{{site}}</a></li>
                    </ul>
                </div> 
            </div>
        </div>
    </section>
</template>

<style lang="scss">
    .footer-links{
    background-image: url(../assets/footer-bg.jpg);
    background-size: cover;
    .container{
        background-image: url(../assets/dc-logo-bg.png);
        background-repeat: no-repeat;
        background-position: right;
        padding: 1.25rem 0;
        .lists{
            display: flex;
            div{
                margin: 1.25rem 1.5625rem 0 0;
                h3{
                    color: white;
                    margin-bottom: 1rem;
                }
                ul{
                    list-style: none;
                    margin-bottom: 1rem;
                    a{
                        text-decoration: none;
                        display: inline-block;
                        color: #797979;
                        padding: .25rem 0;
                    }
                }
            }
        }
    }
}
</style>