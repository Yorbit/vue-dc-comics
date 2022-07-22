<template>
  <footer>
    <section class="container">
        <button>SIGN-UP NOW!</button>
        <nav>
            <span>FOLLOW US</span>
            <a href="#"><img src="../assets/img/footer-periscope.png" alt="periscope"></a>
            <a href="#"><img src="../assets/img/footer-facebook.png" alt="facebook"></a>
            <a href="#"><img src="../assets/img/footer-pinterest.png" alt="pinterest"></a>
            <a href="#"><img src="../assets/img/footer-twitter.png" alt="twitter"></a>
            <a href="#"><img src="../assets/img/footer-youtube.png" alt="youtube"></a>
        </nav>
    </section>
  </footer>
</template>

<script>
export default {
}
</script>

<style lang="scss" scoped>
@import'../styles/colors.scss';
@import'../styles/general.scss';
footer{
    background-color: $footerBg;
    position: relative;
    height: 120px;
    padding: 30px;
    .container{
        display: flex;
        justify-content: space-between;
        width: 1400px;
        margin: 0 auto;
        align-items: center;
        button{
            padding: 20px;
            font-size: 18px;
            border: 2px solid $ShopBg;
            background-color: $footerBg;
            color: white;
        }
        span{
            vertical-align: super;
            font-size: 35px;
            font-weight: bold;
            color: $ShopBg;
            padding: 10px;
        }
        a{
            padding: 15px;
        }
    }
}
</style>