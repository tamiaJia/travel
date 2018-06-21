<template>
  <div>
    <home-header></home-header>
    <home-swiper></home-swiper>
    <div>text</div>
  </div>
</template>
<script type="text/javascript">
import HomeHeader from './components/header'
import HomeSwiper from './components/Swiper'
export default{
  name: 'Home',
  components: {
    HomeHeader,
    HomeSwiper
  }
}
</script>
<style type="text/css">
</style>
