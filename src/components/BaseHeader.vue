<template>
    <header>
        <div class="container">
            <img src="../assets/img/dc-logo.png" alt="">
            <nav>
                <ul>
                    <li v-for="(link, index) in menuHeaderLinks" :key="index">
                        <a :href="link.url" :class="{'active': index == '1'}">
                            {{ link.text }}
                        </a>
                    </li>
                </ul>
            </nav>
        </div>
        <HeaderContent />
    </header>
</template>


<style lang="scss" scoped>
@import'../styles/colors.scss';
@import'../styles/general.scss';

.container{
    justify-content: space-between;
    align-items: center;
    padding: 40px;
    margin: 0 auto;
    display: flex;
    width: 1400px;
}
img{
    height: 120px;
}

.active{
    color: $colorActive;
}
li{
    display: inline-block;
    padding: 10px 10px;
    
    a{
        color: black;
        text-decoration: none;
        font-weight: bold;
    }
}
</style>

<script>
import HeaderContent from './HeaderContent.vue';
export default {
    components: { HeaderContent },
    data: function(){
        return{
            menuHeaderLinks: [
                {
                    text: 'CHARACTERS',
                    url: '#',
                    current: false,
                },
                {
                    text: 'COMICS',
                    url: '#',
                    current: true,
                },
                {
                    text: 'MOVIES',
                    url: '#',
                    current: false,
                },
                {
                    text: 'TV',
                    url: '#',
                    current: false,
                },
                {
                    text: 'GAMES',
                    url: '#',
                    current: false,
                },
                {
                    text: 'COLLECTIBLES',
                    url: '#',
                    current: false,
                },
                {
                    text: 'VIDEOS',
                    url: '#',
                    current: false,
                },
                {
                    text: 'FANS',
                    url: '#',
                    current: false,
                },
                {
                    text: 'NEWS',
                    url: '#',
                    current: false,
                },
                {
                    text: 'SHOP',
                    url: '#',
                    current: false,
                },
                ],  
            }
        }
    }
</script>