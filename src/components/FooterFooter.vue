<script>
export default {
  name:"FooterFooter"
}
</script>

<template>
   <section class="footer-footer">
        <div class="container">
            <button>SIGN UP NOW!</button>
            <div class="socials">
                <span>FOLLOW US</span>
                <img src="../assets/footer-facebook.png" alt="facebook">
                <img src="../assets/footer-twitter.png" alt="twitter">
                <img src="../assets/footer-youtube.png" alt="youtube">
                <img src="../assets/footer-pinterest.png" alt="pinterest">
                <img src="../assets/footer-periscope.png" alt="periscope">
            </div>
        </div>
    </section>
</template>

<style lang="scss">
    .footer-footer{
        background-color: #303030;
        padding: 1.25rem 0;
        button{
            background-color: transparent;
            font-size: 1.125rem;
            font-weight: bold;
            color: white;
            padding: .625rem;
            border: .125rem solid var(--primary-color);
            cursor: pointer;
        }
        .socials{
            display: flex;
            align-items: center;
            color: var(--primary-color);
            font-size: 1.25rem;
            font-weight: bold;
            min-width: 22.5rem;
            justify-content: space-between;
        }
    }
</style>