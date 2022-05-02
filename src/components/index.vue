<template>
  <!-- HEADER -->
  <dHeader />

  <!-- CAROUSEL -->
  <div class="carousel_news">
    <div class="container">
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
  </div>

  <!-- PRODUCT_HOT -->
  <section class="product_hot">
    <div class="container">
      <div class="row">
        <div class="col-lg-4 col-md-12 col-sm-12 col-12 product_hot_item">
          <div class="card">
            <div class="card-body">
              <span>Hot</span>
              <p>SẢN PHẨM NỔI BẬT</p>
            </div>
            <div class="card-img-bottom">
              <img
                src="../assets/products_hot/product_hot1.jpg"
                alt="Card image"
              />
            </div>
          </div>
        </div>
        <div class="col-lg-4 col-md-12 col-sm-12 col-12 product_hot_item">
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
        </div>
        <div class="col-lg-4 col-md-12 col-sm-12 col-12 product_hot_item">
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
        </div>
      </div>
    </div>
  </section>

  <!-- TOP_SEARCH -->
  <section class="top_search">
    <div class="container">
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
    </div>
  </section>

  <!-- PRODUCTS_BEST_SELLER -->
  <section class="products_best_seller">
    <div class="container">
      <div class="products_best_seller_title">
        <h1>
          SẢN PHẨM NỔI BẬT
          <button>
            <img
              src="../assets/products_best_seller/icon_previous.png"
              alt=""
            />
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
    </div>
  </section>

  <!-- BANNER 2 -->
  <section class="content banner_2">
    <img src="../assets/banners/Banner-2.jpg" alt="" />
  </section>

  <!-- PHONE -->
  <section class="products_best_seller phone">
    <div class="container">
      <div class="products_best_seller_title_phone">
        <h1>ĐIỆN THOẠI</h1>
        <p>Các sản phẩm điện thoại do Nam Việt cung cấp mới nhất</p>
      </div>

      <div class="products_best_seller_list">
        <div class="row">
          <ProductItem />
        </div>
      </div>
    </div>
  </section>

  <!-- TABLET -->
  <section class="products_best_seller phone">
    <div class="container">
      <div class="products_best_seller_title_phone">
        <h1>MÁY TÍNH BẢNG</h1>
        <p>Các sản phẩm máy tính bảng do Nam Việt cung cấp mới nhất</p>
      </div>

      <div class="products_best_seller_list">
        <div class="row">
          <ProductItem />
        </div>
      </div>
    </div>
  </section>

  <!-- LAPTOP -->
  <section class="products_best_seller phone">
    <div class="container">
      <div class="products_best_seller_title_phone">
        <h1>MÁY TÍNH APPLE</h1>
        <p>Các sản phẩm máy tính do Nam Việt cung cấp mới nhất</p>
      </div>

      <div class="products_best_seller_list">
        <div class="row">
          <ProductItem />
        </div>
      </div>
    </div>
  </section>

  <!-- OTHER_PRODUCT -->
  <section class="products_best_seller phone">
    <div class="container">
      <div class="products_best_seller_title_phone">
        <h1>SẢN PHẨM KHÁC</h1>
      </div>

      <div class="products_best_seller_list" style="margin-top: 20px">
        <div class="row">
          <ProductItem />
        </div>
      </div>
    </div>
  </section>

  <!-- BANNER 3 -->
  <section class="container">
    <div class="banner_3">
      <div class="banner_3_title">
        <h1>TAI NGHE</h1>
        <h1>NHÃN HÀNG NỔI TIẾNG</h1>
      </div>
      <BannerItem />
    </div>
  </section>

  <!-- BANNER 4 -->
  <section class="container">
    <div class="banner_3 banner_4">
      <div class="banner_3_title">
        <h1>ĐIỆN THOẠI</h1>
        <h1>NHÃN HÀNG NỔI TIẾNG</h1>
      </div>
      <BannerItem />
    </div>
  </section>

  <section-vue title="d"></section-vue>
</template>

<script>
import dHeader from "./dHeader.vue";
import ProductItem from "./productItem.vue";
import BannerItem from "./Banner.vue";
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
    BannerItem,
    Swiper,
    SwiperSlide,
    SectionVue,
  },
  setup() {
    return {
      modules: [Autoplay, Pagination, Navigation],
      images: [
        "../assets/banner_3/airpods.png",
        "../assets/banner_3/airpods.png",
        "../assets/banner_3/airpods.png",
      ],
    };
  },
};
</script>

<style></style>
