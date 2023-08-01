<template>
  <div class="container categories mt-4">
    <div class="row">
      <h3>الفئات</h3>

      <swiper
        :slidesPerView="8.5"
        :pagination="{
          clickable: true,
        }"
        :modules="modules"
        :breakpoints="{
          '375': {
            slidesPerView: 3.3,
            spaceBetween: 10,
          },

          '480': {
            slidesPerView: 3.5,
            spaceBetween: 10,
          },
          '640': {
            slidesPerView: 4.5,
            spaceBetween: 10,
          },
          '767':{
             slidesPerView: 5.5,
            spaceBetween: 10,
          },
          '992': {
            slidesPerView: 7.5,
            spaceBetween: 5,
          },
          '1199': {
            slidesPerView: 8.5,
            spaceBetween: 5,
          },
        }"
        class="mySwiper"
      >
        <swiper-slide
          class="swiper-slide"
          v-for="(item, index) in Categories"
          :key="index"
          ><div class="circle">
            <span>
              <svg
                width="47"
                height="49"
                viewBox="0 0 47 49"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <g clip-path="url(#clip0_11_2086)">
                  <path
                    d="M23.1222 7.96614L42.6174 19.0888H47L37.4791 3.75755H33.0965V-0.00012207H28.1093V3.75755H9.5209L0 19.5398H4.98714L23.1222 7.96614ZM43.373 22.3956L23.2733 11.2729L4.08039 22.5459V43.7391H1.05788V48.9999H45.9421V43.7391H43.2219V22.3956H43.373ZM13.299 36.6747H7.55627V26.9048H13.4502L13.299 36.6747ZM27.3537 44.0398H19.1929V27.2054H27.3537V44.0398ZM39.8971 36.6747H34.0032V26.9048H39.8971V36.6747Z"
                    fill="#0070C0"
                  />
                </g>
                <defs>
                  <clipPath id="clip0_11_2086">
                    <rect width="47" height="49" fill="white" />
                  </clipPath>
                </defs>
              </svg>
            </span>
          </div>
          <a href="#">{{ item.title }}</a>
        </swiper-slide>
      </swiper>
    </div>
  </div>
</template>
<script>
import { Swiper, SwiperSlide } from "swiper/vue";

// Import Swiper styles
import "swiper/css";

import "swiper/css/pagination";

// import "./style.css";

// import required modules
import { Pagination } from "swiper/modules";

export default {
  components: {
    Swiper,
    SwiperSlide,
  },
  data() {
    return {
      Categories: [
        { id: 1, title: " السيارات" },
        { id: 1, title: "العقار" },
        { id: 2, title: " الأجهزة" },
        { id: 3, title: "أثاث" },
        { id: 4, title: " وحيوانات وطيور " },
        { id: 5, title: "مستلزمات شخصية " },
        { id: 6, title: "أطعمة ومشروبات" },
        { id: 7, title: "وظائف" },
        { id: 8, title: "برمجة وتصاميم" },
        { id: 9, title: "مكتبة وفنون" },
        { id: 10, title: "صيد ورحلات " },
        { id: 11, title: "العقار" },
        { id: 12, title: "العقار" },
        { id: 13, title: "العقار" },
        { id: 14, title: "العقار" },
        { id: 15, title: "العقار" },
      ],
    };
  },
  setup() {
    return {
      modules: [Pagination],
    };
  },
};
</script>
