<template>
  <section class="container-fluid my-5">
    <h2>Top Movies</h2>
    <swiper
      :effect="'coverflow'"
      :grabCursor="true"
      :centeredSlides="true"
      :slidesPerView="3"
      :loop="true"
      :coverflowEffect="{
        rotate: 50,
        stretch: 1,
        depth: 50,
        modifier: 1,
        slideShadows: true,
      }"
      :pagination="false"
      class="mySwiper mt-5 w-100"
    >
      <swiper-slide v-for="item in 10" :key="item">
        <div
          class="swiper-slide swiper-bg"
          :style="{'background-image' :'url(../../src/assets/images/movies/0' + item +'.jpg)'}"
        >
          <!-- <img alt="" class="slide-img" :src="'../../src/assets/images/movies/0'+ item +'.jpg'" /> -->
          <div class="top-badge">
            <div class="video-badge">
              <img
                alt=""
                class="img-fluid"
                src="../../assets/images/top-movies.png"
              />
            </div>
          </div>
          <div class="content">
            <p
              class="title"
              data-swiper-parallax="-30%"
              data-swiper-parallax-scale=".7"
            >
              Romantic world
            </p>
            <span class="caption mb-4" data-swiper-parallax="-20%">
              Lorem Ipsum has been the industry's standard dummy text ever since
              the 1500s, when an unknown printer took a galley of type and
              scrambled it to make a type specimen book.</span
            >
            <div
              class="slider-buttons d-flex align-items-center"
              data-swiper-parallax="-30%"
              data-swiper-parallax-scale=".7"
            >
              <a class="btn hvr-sweep-to-right" href="" tabindex="0"
                ><i aria-hidden="true" class="fa fa-play mr-2"></i>Play Now</a
              >
              <a class="btn hvr-sweep-to-right ml-3" href="#" tabindex="0"
                ><i class="fas fa-plus mr-2"></i>My List</a
              >
            </div>
          </div>
        </div>
      </swiper-slide>
    </swiper>
  </section>
</template>


<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";

// import Swiper core and required modules
import SwiperCore, { EffectCoverflow, Pagination } from "swiper";

// install Swiper modules
SwiperCore.use([EffectCoverflow, Pagination]);

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  data() {
    return {};
  },
  methods: {},
};
</script>

<style>

</style>