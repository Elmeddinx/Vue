<template>
  <div class="container-fluid mt-5">
    <h2>Popular Movies</h2>

    <swiper
      :slidesPerView="6"
      :spaceBetween="30"
      :pagination="false"
      :loop="true"
      class="mySwiper mt-5"
    >
      <swiper-slide v-for="item in 6" :key="item">
        <div>
          <div class="video-block">
            <div class="video-thumb position-relative thumb-overlay">
              <a href="#"
                ><img
                  alt=""
                  class="img-fluid"
                  :src="'../src/assets/images/latest-aditions/0' + item +'.jpg'"
              /></a>
              <div class="box-content">
                <ul class="icon">
                  <li>
                    <a href="watch-movie.html"><i class="fas fa-play"></i></a>
                  </li>
                  <li>
                    <a href="#"><i class="fas fa-plus"></i></a>
                  </li>
                  <li>
                    <a href="movie-single.html"><i class="fas fa-info"></i></a>
                  </li>
                </ul>
              </div>
              <!-- Box Content End -->
            </div>
            <!-- Video Thumb End -->
            <div class="video-content">
              <h2 class="video-title">
                <a href="movie-single.html">Iron door</a>
              </h2>
              <div class="video-info d-flex align-items-center">
                <span class="video-year">2021</span>
                <span class="video-age">+18</span>
                <span class="video-type">Action</span>
              </div>
            </div>
            <!-- video Content End -->
          </div>
          <!-- video Block End -->
        </div>
      </swiper-slide>
    </swiper>
  </div>
</template>

<script>
// Import Swiper Vue.js components
import { Swiper, SwiperSlide } from "swiper/vue";

// import Swiper core and required modules
import SwiperCore, { FreeMode, Pagination } from "swiper";

// install Swiper modules
SwiperCore.use([FreeMode, Pagination]);

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