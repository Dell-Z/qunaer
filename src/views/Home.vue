/* eslint-disable vue/no-unused-components */
<template>
  <div>
   <HomeHeader></homeHeader>
   <HomeSwiper></HomeSwiper>
  </div>
</template>

<script>
import HomeHeader from '../components/Header'
import HomeSwiper from '../components/Swiper'
export default{
  components:{ HomeHeader,HomeSwiper },
  name: 'Home'
}
</script>
