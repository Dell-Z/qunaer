<template>
  <div class="swiper">
    <swiper
      :options="swiperOption"
      :not-next-tick="notNextTick"
      ref="mySwiper"
    >
      <!-- slides -->
      <swiper-slide
        v-for="banner in banners" :key="banner.id"
      ><img
          :src="banner.url"
          alt=""
          class="swiper-img"
        ></swiper-slide>
      <!-- Optional controls -->
      <div
        class="swiper-pagination"
        slot="pagination"
      ></div>

    </swiper>
  </div>
</template>

<script>
export default {
  name: "HomeSwiper",
  data() {
    return {
      banners: [
        {
          id: "01",
          url: "https://dimg04.c-ctrip.com/images/0zg3j1200001u5mwh89C1.jpg",
        },
        {
          id: "02",
          url: "https://dimg04.c-ctrip.com/images/0zg6h120006wpw7h44591.jpg",
        },
        {
          id: "03",
          url: "https://dimg04.c-ctrip.com/images/0zg0f120007uslhbcB36B.jpg",
        },
      ],
      swiperOption: {
        pagination: ".swiper-pagination",
        loop: true,
        autoplay:3000
      },
    };
  },
};
</script>

<style lang="stylus" scoped>
.swiper>>> .swiper-pagination-bullet-active
  background: #fff
.swiper-img
  width: 100%
  height 100%
</style>