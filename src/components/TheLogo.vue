<template>
  <div class="logo">
    <img src="@/assets/img/logo.png" alt="logo" />
    <div class="logo__container">
      <h2 class="logo__title">Vue sneakers</h2>
      <p class="logo__description">Магазин лучших кроссовок</p>
    </div>
  </div>
</template>

<script setup>
</script>

<style lang="scss" scoped>
.logo {
  display: flex;
  align-items: center;
  & img {
    width: 60px;
    height: 60px;
    margin-right: 20px;
  }
  &__title,
  &__description {
    margin-top: 5px;
  }
  &__title {
  margin-top: 10px;
    font-size: 24px;
    font-weight: 700;
    text-transform: uppercase;
  }
  &__description {
    color: #9d9d9d;
  }
}
</style>