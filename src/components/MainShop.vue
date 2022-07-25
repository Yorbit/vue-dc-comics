<template>
    <div class="banner-shop">
        <div class="container">
            <div v-for="(link, index) in shopLinks" :key="index">
                <img :src="require(`../assets/img/buy-${link.url}`)" :alt="link.text">
                <a href="#">
                    {{ link.text }}
                </a>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data: function(){
        return{
            shopLinks: [
                {
                    text: 'DIGITAL COMICS',
                    url: 'comics-digital-comics.png'
                },
                {
                    text: 'DC MERCHANDISE',
                    url: 'comics-merchandise.png',
                },
                {
                    text: 'SUBSCRIPTION',
                    url: 'comics-subscriptions.png',
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    url: 'comics-shop-locator.png',
                },
                {
                    text: 'DC POWER VISA',
                    url: 'dc-power-visa.svg',
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>

@import'../styles/colors.scss';
@import'../styles/general.scss';

a{
    color: white;
    text-decoration: none;
    padding: 5px 10px;
}

.banner-shop {
    padding: 40px;
    background-color: $ShopBg;
    position: relative;

    .container {
        justify-content: space-between;
        width: 1300px;
        display: flex;
        margin: 0 auto;
    
        div {
            display: flex;
            align-items: center;
    
            img {
                height: 60px;
            }
        }
    }

}
</style>