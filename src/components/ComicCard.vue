<template>
    <div class="card">
        <div class="card-cover">
            <img :src="imageUrl" :alt="titleComic">
        </div>
        <h5>{{ titleComic }}</h5>
    </div>
</template>

<script>
export default {
    props: {
        imageUrl: String,
        titleComic: String,
    },
}
</script>

<style lang="scss" scoped>
  @import'../styles/colors.scss';

    .card {
        width: calc(100% / 6);
 
        h5 {
            color: white;
            padding: 5px 15px 30px 10px;
            text-transform: uppercase;
        }

        .card-cover {
                padding: 0 10px;
                object-fit: cover;
                object-position: top;
                height: 300px;
        }
    }
</style>