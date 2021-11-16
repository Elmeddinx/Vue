<template>
  <swiper class="mySwiper">
    <swiper-slide>
      <div class="slider-content d-flex justify-content-center bg-img bg-img-1 w-100 h-100">
        <div class="row align-items-center w-75 h-100">
          <div class="col-xl-6 col-lg-12 col-md-12 d-flex flex-column align-items-start">
            <h3 data-animation-in="fadeInUp" data-delay-in="1">
              <span class="badge bg-warning text-dark">New</span>
            </h3>
            <h1 data-animation-in="fadeInUp" data-delay-in="1">Iron door</h1>
            <div
              class="slide-info"
              data-animation-in="fadeInUp"
              data-delay-in="1"
            >
              <span>2021</span> <span class="radius">+18</span>
              <span>2h 6m</span>
            </div>
            <p class="text-left" data-animation-in="fadeInUp" data-delay-in="1">
              Lorem Ipsum is simply dummy text of the printing and typesetting
              industry. Lorem Ipsum has been the industry's standard dummy text
              ever since the 1500s.
            </p>
            <div
              class="slider-buttons d-flex align-items-center"
              data-animation-in="fadeInUp"
              data-delay-in="1"
            >
              <a
                class="btn hvr-sweep-to-right"
                href=""
                tabindex="0"
                ><i aria-hidden="true" class="fa fa-play mr-2"></i>Play Now</a
              >
              <a class="btn hvr-sweep-to-right ml-3" href="#" tabindex="0"
                ><i class="fas fa-plus mr-2"></i>My List</a
              >
            </div>
          </div>
          <!-- Col End -->
        </div>
        <!-- Row End -->
      </div>
    </swiper-slide>
    <swiper-slide>
      <div class="slider-content d-flex justify-content-center bg-img bg-img-2 w-100 h-100">
        <div class="row align-items-center w-75 h-100">
          <div class="col-xl-6 col-lg-12 col-md-12 d-flex flex-column align-items-start">
            <h3 data-animation-in="fadeInUp" data-delay-in="1">
              <span class="badge bg-warning text-dark">New</span>
            </h3>
            <h1 data-animation-in="fadeInUp" data-delay-in="1">Iron door</h1>
            <div
              class="slide-info"
              data-animation-in="fadeInUp"
              data-delay-in="1"
            >
              <span>2021</span> <span class="radius">+18</span>
              <span>2h 6m</span>
            </div>
            <p class="text-left" data-animation-in="fadeInUp" data-delay-in="1">
              Lorem Ipsum is simply dummy text of the printing and typesetting
              industry. Lorem Ipsum has been the industry's standard dummy text
              ever since the 1500s.
            </p>
            <div
              class="slider-buttons d-flex align-items-center"
              data-animation-in="fadeInUp"
              data-delay-in="1"
            >
              <a
                class="btn hvr-sweep-to-right"
                href=""
                tabindex="0"
                ><i aria-hidden="true" class="fa fa-play mr-2"></i>Play Now</a
              >
              <a class="btn hvr-sweep-to-right ml-3" href="#" tabindex="0"
                ><i class="fas fa-plus mr-2"></i>My List</a
              >
            </div>
          </div>
          <!-- Col End -->
        </div>
        <!-- Row End -->
      </div>
    </swiper-slide>
    <swiper-slide>
      <div class="slider-content d-flex justify-content-center bg-img bg-img-3 w-100 h-100">
        <div class="row align-items-center w-75 h-100">
          <div class="col-xl-6 col-lg-12 col-md-12 d-flex flex-column align-items-start">
            <h3 data-animation-in="fadeInUp" data-delay-in="1">
              <span class="badge bg-warning text-dark">New</span>
            </h3>
            <h1 data-animation-in="fadeInUp" data-delay-in="1">Iron door</h1>
            <div
              class="slide-info"
              data-animation-in="fadeInUp"
              data-delay-in="1"
            >
              <span>2021</span> <span class="radius">+18</span>
              <span>2h 6m</span>
            </div>
            <p class="text-left" data-animation-in="fadeInUp" data-delay-in="1">
              Lorem Ipsum is simply dummy text of the printing and typesetting
              industry. Lorem Ipsum has been the industry's standard dummy text
              ever since the 1500s.
            </p>
            <div
              class="slider-buttons d-flex align-items-center"
              data-animation-in="fadeInUp"
              data-delay-in="1"
            >
              <a
                class="btn hvr-sweep-to-right"
                href=""
                tabindex="0"
                ><i aria-hidden="true" class="fa fa-play mr-2"></i>Play Now</a
              >
              <a class="btn hvr-sweep-to-right ml-3" href="#" tabindex="0"
                ><i class="fas fa-plus mr-2"></i>My List</a
              >
            </div>
          </div>
          <!-- Col End -->
        </div>
        <!-- Row End -->
      </div>
    </swiper-slide>

  </swiper>
</template>


<script>
import { Swiper, SwiperSlide } from "swiper/vue";
// Import Swiper styles
import "swiper/css";
export default {
  components: {
    Swiper,
    SwiperSlide,
  },
};
</script>

<style scoped>
.swiper {
  width: 100%;
  height: 100vh;
}

.swiper-slide {
  text-align: center;
  font-size: 18px;
  background: #fff;

  /* Center slide text vertically */
  display: -webkit-box;
  display: -ms-flexbox;
  display: -webkit-flex;
  display: flex;
  -webkit-box-pack: center;
  -ms-flex-pack: center;
  -webkit-justify-content: center;
  justify-content: center;
  -webkit-box-align: center;
  -ms-flex-align: center;
  -webkit-align-items: center;
  align-items: center;
}

.swiper-slide img {
  display: block;
  width: 100%;
  height: 100%;
  object-fit: cover;
}
.bg-img {
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
    position: relative;
}
.bg-img-1 {
        background-image: url("../../assets/images/slider/slider1.jpg");
}
.bg-img-2 {
        background-image: url("../../assets/images/slider/slider2.jpg");
}
.bg-img-3 {
        background-image: url("../../assets/images/slider/slider3.jpg");
}
.bg-img::before {    
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    width: 90%;
    height: 100%;
    background: linear-gradient(90deg, rgb(39 40 41) 0%, rgb(39 40 41) 35%, rgba(83, 100, 141, 0) 100%);
}
</style>
