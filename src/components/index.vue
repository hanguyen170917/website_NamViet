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

  <!-- PRODUCTS_BEST_SELLER -->
  <section class="content products_best_seller">
    <div class="products_best_seller_title">
      <h1>
        SẢN PHẨM NỔI BẬT
        <button>
          <img src="../assets/products_best_seller/icon_previous.png" alt="" />
        </button>
        <button>
          <img src="../assets/products_best_seller/icon_next.png" alt="" />
        </button>
      </h1>
      <p>Các sản phẩm được người dùng đánh giá cao vì chất lượng</p>
    </div>

    <div class="products_best_seller_list">
      <div class="row">
        <ProductItem />
        <ProductItem />
      </div>
    </div>
  </section>

  <!-- BANNER 2 -->
  <section class="content banner_2">
    <img src="../assets/banners/Banner-2.jpg" alt="" />
  </section>

  <!-- PHONE -->
  <section class="content products_best_seller phone">
    <div class="products_best_seller_title_phone">
      <h1>ĐIỆN THOẠI</h1>
      <p>Các sản phẩm điện thoại do Nam Việt cung cấp mới nhất</p>
    </div>

    <div class="products_best_seller_list">
      <div class="row">
        <ProductItem />
      </div>
    </div>
  </section>

  <!-- TABLET -->
  <section class="content products_best_seller phone">
    <div class="products_best_seller_title_phone">
      <h1>MÁY TÍNH BẢNG</h1>
      <p>Các sản phẩm máy tính bảng do Nam Việt cung cấp mới nhất</p>
    </div>

    <div class="products_best_seller_list">
      <div class="row">
        <ProductItem />
      </div>
    </div>
  </section>

  <!-- LAPTOP -->
  <section class="content products_best_seller phone">
    <div class="products_best_seller_title_phone">
      <h1>MÁY TÍNH APPLE</h1>
      <p>Các sản phẩm máy tính do Nam Việt cung cấp mới nhất</p>
    </div>

    <div class="products_best_seller_list">
      <div class="row">
        <ProductItem />
      </div>
    </div>
  </section>

  <!-- OTHER_PRODUCT -->
  <section class="content products_best_seller phone">
    <div class="products_best_seller_title_phone">
      <h1>SẢN PHẨM KHÁC</h1>
    </div>

    <div class="products_best_seller_list" style="margin-top: 20px">
      <div class="row">
        <ProductItem />
      </div>
    </div>
  </section>

  <!-- BANNER 3 -->
  <section class="content">
    <div class="banner_3">
      <div class="banner_3_title">
        <h1>TAI NGHE</h1>
        <h1>NHÃN HÀNG NỔI TIẾNG</h1>
      </div>
      <div class="banner_3_content">
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
              <img src="../assets/banner_3/airpods.png" alt="" />
            </swiper-slide>
            <swiper-slide>
              <img src="../assets/banner_3/airpods.png" alt="" />
            </swiper-slide>
            <swiper-slide>
              <img src="../assets/banner_3/airpods.png" alt="" />
            </swiper-slide>
          </swiper>
        </div>
        <div class="banner_3_content_right">
          <div class="row">
            <div class="brand_item"></div>
            <div class="brand_item"></div>
            <div class="brand_item"></div>
            <div class="brand_item"></div>
            <div class="brand_item"></div>
            <div class="brand_item"></div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section-vue title="d"></section-vue>
</template>

<script>
import dHeader from "./dHeader.vue";
import ProductItem from "./productItem.vue";
import { Swiper, SwiperSlide } from "swiper/vue";
import SectionVue from "./SectionVue.vue";

import "swiper/css";

import "swiper/css/pagination";
import "swiper/css/navigation";

import { Autoplay, Pagination, Navigation } from "swiper";

export default {
  name: "dIndex",

  components: {
    dHeader,
    ProductItem,
    Swiper,
    SwiperSlide,
    SectionVue,
  },
  setup() {
    return {
      modules: [Autoplay, Pagination, Navigation],
    };
  },
};
</script>

<style></style>
