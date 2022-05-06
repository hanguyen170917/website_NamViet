<template>
  <section class="products_best_seller">
    <div class="container">
      <div class="products_best_seller_title">
        <h1>SẢN PHẨM NỔI BẬT</h1>
        <p>Các sản phẩm được người dùng đánh giá cao vì chất lượng</p>
        <div class="btn_products_best_seller">
          <button class="btn_prev">
            <img
              src="../assets/products_best_seller/icon_previous.png"
              alt=""
            />
          </button>
          <button class="btn_next">
            <img src="../assets/products_best_seller/icon_next.png" alt="" />
          </button>
        </div>
      </div>

      <div class="products_best_seller_list">
        <div class="row">
          <ProductItem />
          <ProductItem />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
import ProductItem from "./ProductItem.vue";

import "swiper/css";

import "swiper/css/grid";
import "swiper/css/pagination";

export default {
  name: "featuredProducts",
  components: {
    ProductItem,
  },
};
</script>

<style></style>
