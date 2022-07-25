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
                    text: 'Digital Comics',
                    url: 'comics-digital-comics.png'
                },
                {
                    text: 'DC Merchandise',
                    url: 'comics-merchandise.png',
                },
                {
                    text: 'Subscription',
                    url: 'comics-subscriptions.png',
                },
                {
                    text: 'Comic shop locator',
                    url: 'comics-shop-locator.png',
                },
                {
                    text: 'DC Power Visa',
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