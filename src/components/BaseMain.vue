<template>
    <main>
        <MainShop />
        <div class="content-main">
            <div class="container">
                <ul>
                    <h2>DC COMICS</h2>
                    <li v-for="(comic, index) in ComicsDc" :key="index">
                        <a :href="comic.url">
                            {{ comic.text }}
                        </a>
                    </li>
                    <h2>SHOP</h2>
                    <li v-for="(shop, index) in ShopsDc" :key="index">
                        <a :href="shop.url">
                            {{ shop.text }}
                        </a>
                    </li>
                </ul>
                <ul>
                    <h2>DC</h2>
                    <li v-for="(terms, index) in TermsDc" :key="index">
                        <a :href="terms.url">
                            {{ terms.text }}
                        </a>
                    </li>
                </ul>
                <ul>
                    <h2>Sites</h2>
                    <li v-for="(site, index) in SitesDc" :key="index">
                        <a :href="site.url">
                            {{ site.text }}
                        </a>
                    </li>
                </ul>
                <img class="pos" src="../assets/img/dc-logo-bg.png" alt="">
            </div>
        </div>
    </main>
</template>

<script>
import MainShop from './MainShop.vue';
export default {
    components: { MainShop },
    data: function () {
        return {
            ComicsDc: [
                {
                    text: 'Characters',
                    url: '#',
                },
                {
                    text: 'Comics',
                    url: '#',
                },
                {
                    text: 'Movies',
                    url: '#',
                },
                {
                    text: 'Tv',
                    url: '#',
                },
                {
                    text: 'Games',
                    url: '#',
                },
                {
                    text: 'Videos',
                    url: '#',
                },
                {
                    text: 'News',
                    url: '#',
                },
            ],
            ShopsDc: [
                {
                    text: 'Shop DC',
                    url: '#',
                },
                {
                    text: 'Shop DC Collectibles',
                    url: '#',
                },
            ],
            TermsDc: [
                {
                    text: 'Terms of Use',
                    url: '#',
                },
                {
                    text: 'Privacy Policy (New)',
                    url: '#',
                },
                {
                    text: 'Ad Choices',
                    url: '#',
                },
                {
                    text: 'Advertising',
                    url: '#',
                },
                {
                    text: 'Jobs',
                    url: '#',
                },
                {
                    text: 'Subscriptions',
                    url: '#',
                },
                {
                    text: 'Talent Workshops',
                    url: '#',
                },
                {
                    text: 'CPSC Certificates',
                    url: '#',
                },
                {
                    text: 'Ratings',
                    url: '#',
                },
                {
                    text: 'Shop Help',
                    url: '#',
                },
                {
                    text: 'Contact Us',
                    url: '#',
                },
            ],
            SitesDc: [
                {
                    text: 'DC',
                    url: '#',
                },
                {
                    text: 'Mad Magazine',
                    url: '#',
                },
                {
                    text: 'DC Kids',
                    url: '#',
                },
                {
                    text: 'DC Universe',
                    url: '#',
                },
                {
                    text: 'DC Power Visa',
                    url: '#',
                },
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
@import'../styles/colors.scss';
@import'../styles/general.scss';
.content-main {
    background-image: url('../assets/img/footer-bg.jpg');
    padding: 30px;
    .container{
        position: relative;
        width: 1400px;
        margin: 0 auto;
        display: flex;
        padding-bottom: 20px;
        padding-top: 50px;
        .pos{
            position: absolute;
            top: -90px;
            right: 0;
        }
        ul{
            margin-top: 30px;
            margin-right: 30px;
            h2{
                color: white;
                margin: 10px 0px;
            }
            li{
                list-style: none;
                line-height: 25px;
                font-size: 13px;
                a{
                    color: $ooterColorIcon;
                    text-decoration: none;
                }
            }
        }
    }
}
</style>