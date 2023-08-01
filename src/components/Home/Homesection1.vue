<template>
  <div class="home">
    <div class="container-fluid">
      <div class="row p-0">
        <div class="col-12 p-0">
          <swiper
            :spaceBetween="30"
            :pagination="{
              clickable: true,
            }"
            :modules="modules"
            class="mySwiper"
          >
            <swiper-slide>
              <img src="../../assets/backgroundHome.jpg" class="w-100" />
              <div class="overcolor">
                <div class="container overtext">
                  <div class="row">
                    <div class="col-xxl-7 text-end">
                      <h1>استعد لاكتشاف عالم الفرص والتوفير!</h1>
                      <p class="mt-4 d-none d-md-block">
                        انضم إلينا الآن واستمتع برحلة <br />التسوق الفريدة!
                      </p>
                      <button type="button" class="btn btn-primary mt-lg-4">
                        انضم لنا
                      </button>
                    </div>
                  </div>
                </div>
              </div>
            </swiper-slide>
            <swiper-slide>Slide 2</swiper-slide
            ><swiper-slide>Slide 3</swiper-slide>
          </swiper>
       
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import { Swiper, SwiperSlide } from "swiper/vue";

// Import Swiper styles
import "swiper/css";

import "swiper/css/pagination";

// import './style.css';

// import required modules
import { Pagination } from "swiper/modules";

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Pagination],
    };
  },
};
</script>
