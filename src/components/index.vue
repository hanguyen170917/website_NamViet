<template>
  <!-- HEADER -->
  <Header />

  <HeaderMobile />
  <!-- CAROUSEL -->
  <div class="carousel_news">
    <div class="container">
      <div class="row">
        <div class="col-lg-9 col-sm-12">
          <div class="carousel">
            <swiper
              :spaceBetween="30"
              :centeredSlides="true"
              :autoplay="false"
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
        </div>
        <div class="col-lg-3">
          <div class="news">
            <p>BẢN TIN</p>
            <h1>CÔNG NGHỆ</h1>
            <div class="news_item">
              <img src="../assets/news/news1.jpg" alt="" />
              <span
                >iPhone 13 Pro Max là lựa chọn tốt nhất để người dùng...
              </span>
            </div>
            <div class="news_item">
              <img src="../assets/news/news1.jpg" alt="" />
              <span
                >iPhone 13 Pro Max là lựa chọn tốt nhất để người dùng...
              </span>
            </div>
            <div class="news_item">
              <img src="../assets/news/news1.jpg" alt="" />
              <span
                >iPhone 13 Pro Max là lựa chọn tốt nhất để người dùng...
              </span>
            </div>
            <div class="news_item">
              <img src="../assets/news/news1.jpg" alt="" />
              <span
                >iPhone 13 Pro Max là lựa chọn tốt nhất để người dùng...
              </span>
            </div>
            <div class="news_item">
              <img src="../assets/news/news1.jpg" alt="" />
              <span
                >iPhone 13 Pro Max là lựa chọn tốt nhất để người dùng...
              </span>
            </div>
          </div>
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
          <div class="card product_hot_item_2">
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
        <!-- <div class="top_search_item">
          <span>Top tìm kiếm:</span>
        </div> -->
        <ul>
          <li>
            <div class="top_search_item">
              <span>Top tìm kiếm:</span>
            </div>
          </li>
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
  <section class="container banner_2">
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

  <!-- PRODUCT_SLIDER -->
  <section class="product_slider">
    <div class="row">
      <div class="col-lg-12 col-sm-12">
        <div style="display: flex; align-items: center">
          <div class="prevProductSlider">
            <svg
              width="24"
              height="24"
              viewBox="0 0 24 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M15 18L9 12L15 6"
                stroke="black"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
          </div>
          <swiper
            ref="{swiperRef}"
            :slidesPerView="6"
            :centeredSlides="false"
            :spaceBetween="20"
            :loop="true"
            :loopFillGroupWithBlank="true"
            :navigation="{
              prevEl: '.prevProductSlider',
              nextEl: '.nextProductSlider',
            }"
            :modules="modules"
            class="mySwiper"
          >
            <swiper-slide>
              <div class="product_slider_item">
                <img
                  src="../assets/products_slider/product_slider_1.png"
                  alt="imgBanner1"
                />
              </div>
            </swiper-slide>
            <swiper-slide>
              <div class="product_slider_item">
                <img
                  src="../assets/products_slider/product_slider_1.png"
                  alt="imgBanner1"
                />
              </div>
            </swiper-slide>
            <swiper-slide>
              <div class="product_slider_item">
                <img
                  src="../assets/products_slider/product_slider_1.png"
                  alt="imgBanner1"
                />
              </div>
            </swiper-slide>
            <swiper-slide>
              <div class="product_slider_item">
                <img
                  src="../assets/products_slider/product_slider_1.png"
                  alt="imgBanner1"
                />
              </div>
            </swiper-slide>
            <swiper-slide>
              <div class="product_slider_item">
                <img
                  src="../assets/products_slider/product_slider_1.png"
                  alt="imgBanner1"
                />
              </div>
            </swiper-slide>
            <swiper-slide>
              <div class="product_slider_item">
                <img
                  src="../assets/products_slider/product_slider_1.png"
                  alt="imgBanner1"
                />
              </div>
            </swiper-slide>
            <swiper-slide>
              <div class="product_slider_item">
                <img
                  src="../assets/products_slider/product_slider_1.png"
                  alt="imgBanner1"
                />
              </div>
            </swiper-slide>
            <swiper-slide>
              <div class="product_slider_item">
                <img
                  src="../assets/products_slider/product_slider_1.png"
                  alt="imgBanner1"
                />
              </div>
            </swiper-slide>
          </swiper>
          <div class="nextProductSlider">
            <svg
              width="24"
              height="24"
              viewBox="0 0 24 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                d="M9 18L15 12L9 6"
                stroke="black"
                stroke-width="2"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- QUICK_SEARCH -->
  <section class="quick_search">
    <div class="container">
      <div class="quick_search_title">
        <svg
          width="24"
          height="24"
          viewBox="0 0 24 24"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M21.41 11.58L12.41 2.58C12.05 2.22 11.55 2 11 2H4C2.9 2 2 2.9 2 4V11C2 11.55 2.22 12.05 2.59 12.42L11.59 21.42C11.95 21.78 12.45 22 13 22C13.55 22 14.05 21.78 14.41 21.41L21.41 14.41C21.78 14.05 22 13.55 22 13C22 12.45 21.77 11.94 21.41 11.58ZM5.5 7C4.67 7 4 6.33 4 5.5C4 4.67 4.67 4 5.5 4C6.33 4 7 4.67 7 5.5C7 6.33 6.33 7 5.5 7ZM17.27 15.27L13 19.54L8.73 15.27C8.28 14.81 8 14.19 8 13.5C8 12.12 9.12 11 10.5 11C11.19 11 11.82 11.28 12.27 11.74L13 12.46L13.73 11.73C14.18 11.28 14.81 11 15.5 11C16.88 11 18 12.12 18 13.5C18 14.19 17.72 14.82 17.27 15.27Z"
            fill="black"
          />
        </svg>
        <span>Tìm nhanh</span>
      </div>
      <div class="quick_search_tag">
        <div class="quick_search_tag_item">Loa di động</div>
        <div class="quick_search_tag_item">Tai nghe không dây</div>
        <div class="quick_search_tag_item">Tai nghe không dây</div>
        <div class="quick_search_tag_item">Loa di động</div>
        <div class="quick_search_tag_item">Loa di động</div>
        <div class="quick_search_tag_item">Loa di động</div>
        <div class="quick_search_tag_item">Loa di động</div>
        <div class="quick_search_tag_item">Loa di động</div>
        <div class="quick_search_tag_item">Loa di động</div>
        <div class="quick_search_tag_item">Loa di động</div>
        <div class="quick_search_tag_item">Loa di động</div>
        <div class="quick_search_tag_item">Loa di động</div>
        <div class="quick_search_tag_item">Loa di động</div>
      </div>
    </div>
  </section>

  <!-- FOOTER -->
  <Footer />
  <!-- <section-vue title="d"></section-vue> -->
</template>

<script>
import { ref } from "vue";

import Header from "./Header.vue";
import HeaderMobile from "./HeaderMobile.vue";
import ProductItem from "./ProductItem.vue";
import BannerItem from "./Banner.vue";
import Footer from "./Footer.vue";

import { Swiper, SwiperSlide } from "swiper/vue";
// import SectionVue from "./SectionVue.vue";

import "swiper/css";

import "swiper/css/pagination";
import "swiper/css/navigation";

import { Autoplay, Pagination, Navigation } from "swiper";

export default {
  name: "dIndex",
  components: {
    Header,
    HeaderMobile,
    ProductItem,
    BannerItem,
    Footer,
    Swiper,
    SwiperSlide,
    // SectionVue,
  },
  setup() {
    const images = ref([
      "../assets/banner_3/airpods.png",
      "../assets/banner_3/airpods.png",
      "../assets/banner_3/airpods.png",
    ]);
    return {
      modules: [Autoplay, Pagination, Navigation],
      images,
    };
  },
};
</script>

<style></style>
