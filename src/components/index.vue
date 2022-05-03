<template >
  <!-- HEADER -->
  <dHeader/>

 

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

  <!-- PRODUCT_SLIDER -->
  <section class="product_slider">
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
  <section class="footer">
    <div class="row">
      <div class="col-lg-12 border_bottom_footer">
        <div class="container">
          <div class="row">
            <div class="col-lg-3">
              <div class="footer_top">
                <h1 class="footer_title">TIN TỨC</h1>
                <h4 class="footer_item">Tin tức công nghệ</h4>
                <h4 class="footer_item">Tin tức công nghệ</h4>
              </div>
            </div>
            <div class="col-lg-3">
              <div class="footer_top">
                <h1 class="footer_title">CHÍNH SÁCH</h1>
                <h4 class="footer_item">Chính sách bảo hành</h4>
                <h4 class="footer_item">Chính sách đổi mới sản phẩm</h4>
                <h4 class="footer_item">Chi tiết bảo hành VIP của Samsung</h4>
              </div>
            </div>
            <div class="col-lg-3">
              <div class="footer_top">
                <h1 class="footer_title">HỖ TRỢ</h1>
                <h4 class="footer_item">Hình thức thanh toán</h4>
                <h4 class="footer_item">Tư vấn sản phẩm</h4>
                <div class="social_icon">
                  <svg
                    width="31"
                    height="31"
                    viewBox="0 0 31 31"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M23.2499 2.58325H19.3749C17.6621 2.58325 16.0194 3.26368 14.8082 4.47484C13.597 5.68601 12.9166 7.3287 12.9166 9.04155V12.9165H9.04163V18.0832H12.9166V28.4165H18.0832V18.0832H21.9582L23.2499 12.9165H18.0832V9.04155C18.0832 8.69898 18.2193 8.37044 18.4616 8.12821C18.7038 7.88598 19.0323 7.74989 19.3749 7.74989H23.2499V2.58325Z"
                      stroke="white"
                      stroke-width="1.5"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                    />
                  </svg>
                  <svg
                    width="32"
                    height="31"
                    viewBox="0 0 32 31"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M22.3332 2.58325H9.41661C5.84979 2.58325 2.95831 5.47473 2.95831 9.04155V21.9582C2.95831 25.525 5.84979 28.4165 9.41661 28.4165H22.3332C25.9 28.4165 28.7915 25.525 28.7915 21.9582V9.04155C28.7915 5.47473 25.9 2.58325 22.3332 2.58325Z"
                      stroke="white"
                      stroke-width="1.5"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                    />
                    <path
                      d="M21.0416 14.6861C21.201 15.7611 21.0174 16.859 20.5168 17.8236C20.0163 18.7882 19.2244 19.5704 18.2537 20.059C17.283 20.5476 16.1829 20.7177 15.11 20.545C14.0371 20.3724 13.0459 19.8658 12.2774 19.0974C11.509 18.3289 11.0024 17.3377 10.8298 16.2648C10.6571 15.1919 10.8272 14.0918 11.3158 13.1211C11.8044 12.1504 12.5866 11.3585 13.5512 10.858C14.5158 10.3574 15.6137 10.1738 16.6887 10.3332C17.7852 10.4958 18.8003 11.0068 19.5842 11.7906C20.368 12.5745 20.879 13.5896 21.0416 14.6861Z"
                      stroke="white"
                      stroke-width="1.5"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                    />
                    <path
                      d="M22.9791 8.39575H22.9909"
                      stroke="white"
                      stroke-width="1.5"
                      stroke-linecap="round"
                      stroke-linejoin="round"
                    />
                  </svg>
                  <svg
                    width="32"
                    height="31"
                    viewBox="0 0 32 31"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <g clip-path="url(#clip0_405_1137)">
                      <path
                        d="M29.864 8.29257C29.7106 7.67956 29.3981 7.11789 28.9581 6.66431C28.5181 6.21072 27.9663 5.88127 27.3582 5.70925C25.1365 5.16675 16.2499 5.16675 16.2499 5.16675C16.2499 5.16675 7.3633 5.16675 5.14165 5.76091C4.53359 5.93294 3.98171 6.26239 3.54173 6.71597C3.10175 7.16956 2.78926 7.73122 2.63583 8.34423C2.22923 10.5989 2.03034 12.8861 2.04166 15.1771C2.02717 17.4854 2.22607 19.79 2.63583 22.0617C2.80498 22.6556 3.12447 23.1959 3.56342 23.6304C4.00238 24.0648 4.54596 24.3787 5.14165 24.5416C7.3633 25.1358 16.2499 25.1358 16.2499 25.1358C16.2499 25.1358 25.1365 25.1358 27.3582 24.5416C27.9663 24.3696 28.5181 24.0402 28.9581 23.5866C29.3981 23.133 29.7106 22.5713 29.864 21.9583C30.2675 19.7206 30.4664 17.4509 30.4582 15.1771C30.4727 12.8689 30.2738 10.5642 29.864 8.29257V8.29257Z"
                        stroke="white"
                        stroke-width="1.5"
                        stroke-linecap="round"
                        stroke-linejoin="round"
                      />
                      <path
                        d="M13.3437 19.4006L20.7707 15.1769L13.3437 10.9531V19.4006Z"
                        stroke="white"
                        stroke-width="1.5"
                        stroke-linecap="round"
                        stroke-linejoin="round"
                      />
                    </g>
                    <defs>
                      <clipPath id="clip0_405_1137">
                        <rect
                          width="30.9998"
                          height="30.9998"
                          fill="white"
                          transform="translate(0.75)"
                        />
                      </clipPath>
                    </defs>
                  </svg>
                </div>
              </div>
            </div>
            <div class="col-lg-3">
              <div class="footer_top">
                <h1 class="footer_title">THANH TOÁN</h1>
                <div class="payment">
                  <img src="../assets/footer/payment1.png" alt="" />
                  <img src="../assets/footer/payment2.png" alt="" />
                  <img src="../assets/footer/payment3.png" alt="" />
                </div>
                <div class="certifiation">
                  <img src="../assets/footer/certifiation.png" alt="" />
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div
        class="col-lg-12 border_bottom_footer"
        style="padding-bottom: 52px; padding-top: 25px"
      >
        <div class="container">
          <div class="row">
            <div class="col-lg-3">
              <div class="footer_contact">
                <a href="#" class="logo_footer">
                  <img src="../assets/logo2.png" alt="logo2" />
                </a>
              </div>
            </div>
            <div class="col-lg-3" style="padding-top: 10px">
              <div class="footer_contact">
                <h4 class="footer_item">
                  <svg
                    width="12"
                    height="16"
                    viewBox="0 0 12 16"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M6 0.5C3.0975 0.5 0.75 2.8475 0.75 5.75C0.75 9.6875 6 15.5 6 15.5C6 15.5 11.25 9.6875 11.25 5.75C11.25 2.8475 8.9025 0.5 6 0.5ZM6 7.625C4.965 7.625 4.125 6.785 4.125 5.75C4.125 4.715 4.965 3.875 6 3.875C7.035 3.875 7.875 4.715 7.875 5.75C7.875 6.785 7.035 7.625 6 7.625Z"
                      fill="white"
                    />
                  </svg>
                  <span style="margin-left: 27px"
                    >260 Nam Kỳ Khởi Nghĩa, P.8, Q.3, TP. Hồ Chí Minh</span
                  >
                </h4>
                <h4 class="footer_item">
                  <svg
                    width="18"
                    height="18"
                    viewBox="0 0 18 18"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M15.0075 11.535C14.085 11.535 13.1925 11.385 12.36 11.115C12.0975 11.025 11.805 11.0925 11.6025 11.295L10.425 12.7725C8.3025 11.76 6.315 9.8475 5.2575 7.65L6.72 6.405C6.9225 6.195 6.9825 5.9025 6.9 5.64C6.6225 4.8075 6.48 3.915 6.48 2.9925C6.48 2.5875 6.1425 2.25 5.7375 2.25H3.1425C2.7375 2.25 2.25 2.43 2.25 2.9925C2.25 9.96 8.0475 15.75 15.0075 15.75C15.54 15.75 15.75 15.2775 15.75 14.865V12.2775C15.75 11.8725 15.4125 11.535 15.0075 11.535Z"
                      fill="white"
                    />
                  </svg>

                  <span
                    >(028) 3 9320660 <br />
                    0903669949 <br />
                    Fax:(028) 3 9322792</span
                  >
                </h4>
              </div>
            </div>
            <div class="col-lg-3" style="padding-top: 10px">
              <div class="footer_contact">
                <h4 class="footer_item">
                  <svg
                    width="18"
                    height="18"
                    viewBox="0 0 18 18"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M15 3H3C2.175 3 1.5075 3.675 1.5075 4.5L1.5 13.5C1.5 14.325 2.175 15 3 15H15C15.825 15 16.5 14.325 16.5 13.5V4.5C16.5 3.675 15.825 3 15 3ZM15 6L9 9.75L3 6V4.5L9 8.25L15 4.5V6Z"
                      fill="white"
                    />
                  </svg>

                  <span>info@namvietmobile.com</span>
                </h4>
                <h4 class="footer_item">
                  <svg
                    width="16"
                    height="16"
                    viewBox="0 0 16 16"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      d="M8 0.5C3.875 0.5 0.5 3.875 0.5 8C0.5 12.125 3.875 15.5 8 15.5C12.125 15.5 15.5 12.125 15.5 8C15.5 3.875 12.125 0.5 8 0.5ZM11.15 11.15L7.25 8.75V4.25H8.375V8.15L11.75 10.175L11.15 11.15Z"
                      fill="white"
                    />
                  </svg>
                  <span
                    >Thứ 2 đến thứ 7 từ: 08h-20h30 Chủ nhật từ: 08h-18h</span
                  >
                </h4>
              </div>
            </div>
            <div class="col-lg-3" style="padding-top: 20px">
              <div class="footer_contact">
                <input type="text" placeholder="mail..." />
                <button class="btn btnSend">GỬI</button>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="col-lg-12 border_bottom_footer">
        <div class="container">
          <div class="footer_menu">
            <ul>
              <li>Trang chủ</li>
              <li>Sản phẩm</li>
              <li>Tin tức</li>
              <li>Chính sách</li>
              <li>Hỗ trợ</li>
              <li>Thanh toán</li>
            </ul>
          </div>
        </div>
      </div>
      <div class="col-lg-12">
        <div class="footer_copyRight">
          <p>Copyright © 2021 by Smart Digi-tech</p>
        </div>
      </div>
    </div>
  </section>
  <!-- <section-vue title="d"></section-vue> -->
</template>

<script>
import { ref } from 'vue';

import dHeader from "./dHeader.vue";
import ProductItem from "./productItem.vue";
import BannerItem from "./Banner.vue";

import { Swiper, SwiperSlide } from "swiper/vue";
// import SectionVue from "./SectionVue.vue";

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
