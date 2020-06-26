<template>
  <div class="wrapper">
    <swiper class="swiper" :options="swiperOption">
      <swiper-slide class="swiper-img">1</swiper-slide>
      <swiper-slide class="swiper-img">2</swiper-slide>
      <swiper-slide class="swiper-img">3</swiper-slide>
      <swiper-slide class="swiper-img">4</swiper-slide>
      <div class="swiper-pagination" slot="pagination"></div>
    </swiper>
  </div>
</template>
<script>
  import { Swiper, SwiperSlide } from 'vue-awesome-swiper'
  import 'swiper/css/swiper.css'

  export default {
    components: {
      Swiper,
      SwiperSlide
    },
    data() {
      return {
        swiperOption: {
          spaceBetween: 30,
          centeredSlides: true,
          autoplay: {
            delay: 2500,
            disableOnInteraction: false
          },
          pagination: {
            el: '.swiper-pagination',
            clickable: true
          }
        }
      }
    }
  }
</script>
<style scoped>
.wrapper {
  width: 100%;
  height: 0;
  background: #fff;
}
.swiper-img{
    width: 100%;
    height: 3rem;
    background-color: #1062c5;
}
</style>