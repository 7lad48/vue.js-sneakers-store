<template>
    <Header/>
    <Banner/>
    <Cart/>
    <main class="main">
      <router-view/>
    </main>
</template>

<script setup>
import Header from '@/components/TheHeader'
import Cart from '@/components/cart/TheCart'
import Banner from '@/components/TheBanner'

</script>

<style lang="scss" scoped>
.main {
  flex: 1;
  padding: 60px;
}

@media (max-width: 768px) {
  .main {
    padding: 20px;
  }
}
@media (max-width: 425px) {
  .main {
    padding: 15px 10px;
  }
}
</style>