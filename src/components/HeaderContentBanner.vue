<template>
    <div class="jumbo">
        <div class="header-container">
            <p>CURRENT SERIES</p>
        </div>
    </div>
</template>

<script>
export default {
}
</script>

<style lang="scss" scoped>

  @import'../styles/colors.scss';

    .jumbo{
    background-image: url('../assets/img/jumbotron.jpg');
    height: 400px;
      p{
          background-color: $ShopBg;
          color: white;
          position: relative;
          font-size: 22px;
          top: 375px;
          left: 220px;
          width: 17%;
          font-weight: bold;
          padding: 10px 25px;
       }
    }
</style>