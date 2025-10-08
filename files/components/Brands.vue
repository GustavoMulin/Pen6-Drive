<template>
  <section class="brand-one">
    <p class="text-center">Nossos clientes</p>
      <div class="brand-one__carousel">

        <swiper :options="swiperOptions">
          <swiper-slide v-for="(logo, index) in logos" :key="index">
            <div class="item">
            <img :src="logo" alt="">
            </div><!-- /.item -->
          </swiper-slide>
        </swiper>

      </div>
  </section>
</template>


<script>
  import { Swiper, SwiperSlide, directive } from 'vue-awesome-swiper';
  import 'swiper/css/swiper.css';

  export default {
    name: "Brands",
    components: {
      Swiper,
      SwiperSlide
    },
    directives: {
      swiper: directive
    },
    data() {
      return {
        swiperOptions: {
          slidesPerView : 'auto',
          loop: true,
          speed: 6000,
          spaceBetween : 15,
          allowTouchMove: false,
          autoplay: {
						delay: 0,
						disableOnInteraction: false
					},
          // Responsive breakpoints
          breakpoints: {
            1024:{
              slidesPerView : 5
            },
            768:{
              slidesPerView : 4
            },
            640:{
              slidesPerView : 3
            },
            320:{
              slidesPerView : 2
            }
          }
        },

        logos: [
          '/assets/images/resources/1.png',
          '/assets/images/resources/2.png',
          '/assets/images/resources/3.png',
          '/assets/images/resources/4.png',
          '/assets/images/resources/5.png',
          '/assets/images/resources/6.png',
          '/assets/images/resources/7.png',
        ]
      }
    },
  }
</script>

<style scoped>

:deep(.swiper-wrapper) {
  transition-timing-function: linear !important;
}
</style>
