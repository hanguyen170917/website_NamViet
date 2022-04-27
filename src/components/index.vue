<template>
  <!-- HEADER -->
  <dHeader />

  <!-- CAROUSEL -->
  <div class="content carousel_news">
    <div class="carousel">
      <swiper
        :spaceBetween="30"
        :centeredSlides="true"
        :autoplay="{
          delay: 4000,
          disableOnInteraction: false,
        }"
        :pagination="true"
        :navigation="true"
        :modules="modules"
        class="mySwiper"
      >
        <swiper-slide>
          <img src="../assets/banners/banner1.jpg" alt="imgBanner1" />
        </swiper-slide>
        <swiper-slide>
          <img src="../assets/banners/banner1.jpg" alt="imgBanner1" />
        </swiper-slide>
        <swiper-slide>
          <img src="../assets/banners/banner1.jpg" alt="imgBanner1" />
        </swiper-slide>
        <swiper-slide>
          <img src="../assets/banners/banner1.jpg" alt="imgBanner1" />
        </swiper-slide>
      </swiper>
    </div>
    <div class="news">
      <p>BẢN TIN</p>
      <h1>CÔNG NGHỆ</h1>
      <div class="news_item">
        <img src="../assets/news/news1.jpg" alt="" />
        <span>iPhone 13 Pro Max là lựa chọn tốt nhất để người dùng... </span>
      </div>
      <div class="news_item">
        <img src="../assets/news/news1.jpg" alt="" />
        <span>iPhone 13 Pro Max là lựa chọn tốt nhất để người dùng... </span>
      </div>
      <div class="news_item">
        <img src="../assets/news/news1.jpg" alt="" />
        <span>iPhone 13 Pro Max là lựa chọn tốt nhất để người dùng... </span>
      </div>
      <div class="news_item">
        <img src="../assets/news/news1.jpg" alt="" />
        <span>iPhone 13 Pro Max là lựa chọn tốt nhất để người dùng... </span>
      </div>
      <div class="news_item">
        <img src="../assets/news/news1.jpg" alt="" />
        <span>iPhone 13 Pro Max là lựa chọn tốt nhất để người dùng... </span>
      </div>
    </div>
  </div>

  <!-- PRODUCT_HOT -->
  <section class="content product_hot">
    <div class="card">
      <div class="card-body">
        <span>Hot</span>
        <p>SẢN PHẨM NỔI BẬT</p>
      </div>
      <img
        class="card-img-bottom"
        src="../assets/products_hot/product_hot1.jpg"
        alt="Card image"
      />
    </div>
    <div class="card" style="margin: 0 10px">
      <div class="card-body">
        <span>?%</span>
        <p>SẢN PHẨM KHUYẾN MÃI</p>
      </div>
      <img
        class="card-img-bottom"
        src="../assets/products_hot/product_hot2.jpg"
        alt="Card image"
      />
    </div>
    <div class="card">
      <div class="card-body">
        <span>New</span>
        <p>SẢN PHẨM MỚI</p>
      </div>
      <img
        class="card-img-bottom"
        src="../assets/products_hot/product_hot3.jpg"
        alt="Card image"
      />
    </div>
  </section>

  <!-- TOP_SEARCH -->
  <section class="content top_search">
    <div class="top_search_content">
      <div class="top_search_item">
        <span>Top tìm kiếm:</span>
      </div>
      <ul>
          <li>#Loadidong</li>
          <li>#USB</li>
          <li>#Chuotkhongdayapple</li>
          <li>#iphone13</li>
          <li>#iphone11</li>
          <li>#macbookM12021</li>
          <li>#oplungiphone</li>
        </ul>
    </div>
  </section>
</template>

<script>
import dHeader from "./dHeader.vue";
import { Swiper, SwiperSlide } from "swiper/vue";

import "swiper/css";

import "swiper/css/pagination";
import "swiper/css/navigation";

import { Autoplay, Pagination, Navigation } from "swiper";

export default {
  name: "dIndex",

  components: {
    dHeader,
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
