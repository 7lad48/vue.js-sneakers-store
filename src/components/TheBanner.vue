<script setup>

</script>

<template>
  <div class="banner__wrapper">
    <div class="banner__text">Скоро в продаже</div>
    <div class="banner__picture">
      <img src="@/assets/img/banner.png" alt="logo"/>
    </div>
  </div>

</template>

<style scoped lang="scss">
  @import "src/assets/scss/adaptiveFont";
  .banner__wrapper{
    background: rgb(143, 174, 248);
    margin: 20px 25px;
    border-radius: 25px;
    display: flex;
    justify-content: center;
    align-items: center;
    .banner__text{
      @include adaptive-font(55, 20, 1450);
      font-weight: 700;
      white-space: nowrap;
      color: #fff;
      font-style: italic;
      margin-left: 20px;
    }
    .banner__picture{
      animation: pictureAnimation 3s infinite alternate;
    }
    .banner__picture img{
      max-height: 250px;
      transform: rotate(-20deg);
      position: relative;
    }
    @keyframes pictureAnimation {
      0% {
        transform: translateY(10px);
      }
      100% {
        transform: translateY(-20px);
      }
    }
  }
</style>