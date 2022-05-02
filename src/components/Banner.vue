<template>
  <div class="banner_3_content">
    <div class="row">
      <div class="col-lg-3 col-md-12 col-sm-12 col-12">
        <div class="banner_3_content_left">
          <h1>Thương hiệu</h1>
          <img src="../assets/banner_3/logo_apple.png" alt="" />
          <p class="product_type">Tai nghe không dây</p>
          <h1>Apple Airpods 3</h1>
          <p class="price">Giá: 2.000.000 đ</p>
          <a href="#">
            Mua ngay
            <img src="../assets/banner_3/icon_buy_now.png" alt="" />
          </a>
        </div>
      </div>
      <div class="col-lg-6 col-md-12 col-sm-12 col-12">
        <div class="banner_3_content_center">
          <swiper
            :spaceBetween="30"
            :centeredSlides="true"
            :pagination="{
              clickable: true,
            }"
            :autoplay="{
              delay: 4000,
              disableOnInteraction: false,
            }"
            :navigation="true"
            :modules="modules"
            class="mySwiper"
          >
            <swiper-slide>
              <div class="ratio_custom">
                <img src="../assets/banner_3/airpods.png" alt="" />
              </div>
            </swiper-slide>
            <swiper-slide>
              <div class="ratio_custom">
                <img src="../assets/banner_3/airpods.png" alt="" />
              </div>
            </swiper-slide>
            <swiper-slide>
              <div class="ratio_custom">
                <img src="../assets/banner_3/airpods.png" alt="" />
              </div>
            </swiper-slide>
          </swiper>
        </div>
      </div>
      <div class="col-lg-3 col-md-12 col-sm-12 col-12" style="padding: 0">
        <div class="banner_3_content_right">
          <div class="row">
            <div class="col-lg-6 col-md-12 col-sm-12 col-12">
              <div class="brand_item">
                <img src="../assets/banner_3/brand_1.png" alt="" />
              </div>
            </div>
            <div class="col-lg-6 col-md-12 col-sm-12 col-12">
              <div class="brand_item">
                <img src="../assets/banner_3/brand_2.png" alt="" />
              </div>
            </div>
            <div class="col-lg-6 col-md-12 col-sm-12 col-12">
              <div class="brand_item">
                <img src="../assets/banner_3/brand_3.png" alt="" />
              </div>
            </div>
            <div class="col-lg-6 col-md-12 col-sm-12 col-12">
              <div class="brand_item">
                <img src="../assets/banner_3/brand_4.png" alt="" />
              </div>
            </div>
            <div class="col-lg-6 col-md-12 col-sm-12 col-12">
              <div class="brand_item">
                <img src="../assets/banner_3/brand_5.png" alt="" />
              </div>
            </div>
            <div class="col-lg-6 col-md-12 col-sm-12 col-12">
              <div class="brand_item">
                <img src="../assets/banner_3/brand_6.png" alt="" />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { Swiper, SwiperSlide } from "swiper/vue";
import "swiper/css";

import "swiper/css/pagination";
import "swiper/css/navigation";

import { Autoplay, Pagination, Navigation } from "swiper";

export default {
  name: "bannerItem",

  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [Autoplay, Pagination, Navigation],
    };
  },
};
</script>

<style></style>
