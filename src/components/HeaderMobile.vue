<template>
  <div class="header_nav header_mobile">
    <header class="header">
      <div class="container">
        <div class="contact">
          <img src="../assets/icon/phone-contact.png" alt="phone contact" />
          <span>Hotline: (028) 3 9320660 - 0903669949</span>
        </div>
        <section class="menu">
          <div class="container" ref="navContent">
            <div class="header_mobile_nav">
              <div class="header_mobile_nav_left">
                <div class="toggler">
                  <button class="btnToggle" @click="toggleMenu(1)">
                    <svg
                      width="26"
                      height="26"
                      viewBox="0 0 26 26"
                      fill="none"
                      xmlns="http://www.w3.org/2000/svg"
                    >
                      <path
                        d="M2.16663 21.6668H23.8333V17.3335H2.16663V21.6668ZM4.33329 18.4168H6.49996V20.5835H4.33329V18.4168ZM2.16663 4.3335V8.66683H23.8333V4.3335H2.16663ZM6.49996 7.5835H4.33329V5.41683H6.49996V7.5835ZM2.16663 15.1668H23.8333V10.8335H2.16663V15.1668ZM4.33329 11.9168H6.49996V14.0835H4.33329V11.9168Z"
                        fill="white"
                      />
                    </svg>
                  </button>
                </div>
                <div class="logo">
                  <a href="#">
                    <img src="../assets/logo2.png" alt="logo2" />
                  </a>
                </div>
              </div>
              <div class="header_mobile_nav_right">
                <div class="search_mobile">
                  <a href="#" @click="showFormSearch()">
                    <svg
                      width="24"
                      height="24"
                      viewBox="0 0 24 24"
                      fill="none"
                      xmlns="http://www.w3.org/2000/svg"
                    >
                      <path
                        d="M11 19C15.4183 19 19 15.4183 19 11C19 6.58172 15.4183 3 11 3C6.58172 3 3 6.58172 3 11C3 15.4183 6.58172 19 11 19Z"
                        stroke="white"
                        stroke-width="2"
                        stroke-linecap="round"
                        stroke-linejoin="round"
                      />
                      <path
                        d="M21 20.9999L16.65 16.6499"
                        stroke="white"
                        stroke-width="2"
                        stroke-linecap="round"
                        stroke-linejoin="round"
                      />
                    </svg>
                  </a>
                </div>
                <div class="cart">
                  <img src="../assets/icon/cart.png" alt="iconCart" />
                </div>
                <div class="acount">
                  <img src="../assets/icon/user.png" alt="iconCart" />
                </div>
              </div>
            </div>
          </div>
        </section>
        <div class="header_mobile_nav_search" v-if="isShowFormSearch">
          <div class="search">
            <input
              type="text"
              class="form-control"
              id="txtSearch"
              placeholder="Tìm kiếm ...."
            />
          </div>
        </div>
      </div>
    </header>
  </div>
  <div id="menu__dropdown" class="container" ref="menuDropdown">
    <div class="menu_dropdown" v-if="isShowMenu">
      <div class="row">
        <div class="col-6 menu_dropdown_mobile_left">
          <div class="nav_left">
            <div
              class="nav_left_item"
              @click="toggleMenu(1)"
              :class="{ nav_left_item_active: activeMenu === 1 }"
            >
              <p>ĐIỆN THOẠI</p>
            </div>
            <div
              class="nav_left_item"
              @click="toggleMenu(2)"
              :class="{ nav_left_item_active: activeMenu === 2 }"
            >
              <p>MÁY TÍNH BẢNG</p>
            </div>
            <div
              class="nav_left_item"
              @click="toggleMenu(3)"
              :class="{ nav_left_item_active: activeMenu === 3 }"
            >
              <p>WATCH</p>
            </div>
            <div
              class="nav_left_item"
              @click="toggleMenu(4)"
              :class="{ nav_left_item_active: activeMenu === 4 }"
            >
              <p>MÁY TÍNH APPLE</p>
            </div>
            <div
              class="nav_left_item"
              @click="toggleMenu(5)"
              :class="{ nav_left_item_active: activeMenu === 5 }"
            >
              <p>LOA DI ĐỘNG</p>
            </div>
            <div
              class="nav_left_item"
              @click="toggleMenu(6)"
              :class="{ nav_left_item_active: activeMenu === 6 }"
            >
              <p>TAI NGHE</p>
            </div>
            <div
              class="nav_left_item"
              @click="toggleMenu(7)"
              :class="{ nav_left_item_active: activeMenu === 7 }"
            >
              <p>SẢN PHẨM APPLE</p>
            </div>
            <div
              class="nav_left_item"
              @click="toggleMenu(8)"
              :class="{ nav_left_item_active: activeMenu === 8 }"
            >
              <p>BALO</p>
            </div>
          </div>
        </div>
        <div class="col-6 menu_dropdown_mobile_right">
          <div class="content_right">
            <div class="brands_list">
              <div class="row">
                <BrandItem />
                <BrandItem />
                <BrandItem />
                <BrandItem />
                <BrandItem />
                <BrandItem />
                <BrandItem />
                <BrandItem />
                <BrandItem />
                <BrandItem />
                <BrandItem />
                <BrandItem />
              </div>
            </div>

            <!-- <div class="quick_search">
            <div class="row">
              <QuickSearchItem />
              <QuickSearchItem />
              <QuickSearchItem />
              <QuickSearchItem />
              <QuickSearchItem />
              <QuickSearchItem />
              <QuickSearchItem />
            </div>
          </div> -->
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { ref, onBeforeUnmount, onMounted } from "vue";

import BrandItem from "./Brand.vue";
// import QuickSearchItem from "./QuickSearch.vue";

export default {
  name: "HeaderMobile",
  components: {
    BrandItem,
    // QuickSearchItem,
  },

  setup() {
    const isShowMenu = ref(false);
    const activeMenu = ref(1);
    const navContent = ref(null);
    const menuDropdown = ref(null);
    const isShowFormSearch = ref(false);

    function toggleMenu(id) {
      if (activeMenu.value === id) {
        isShowMenu.value = !isShowMenu.value;
        return;
      }
      activeMenu.value = id;
    }

    const clickOutside = (event) => {
      if (navContent.value.contains(event.target)) return;
      if (menuDropdown.value && menuDropdown.value.contains(event.target))
        return;
      isShowMenu.value = false;
    };
    onMounted(() => {
      document.querySelector("html").addEventListener("click", clickOutside);
    });
    onBeforeUnmount(() => {
      document.querySelector("html").removeEventListener("click", clickOutside);
    });

    function showFormSearch() {
      isShowFormSearch.value = !isShowFormSearch.value;
    }
    return {
      isShowMenu,
      toggleMenu,
      activeMenu,
      navContent,
      menuDropdown,
      showFormSearch,
      isShowFormSearch,
    };
  },
};
</script>

<style></style>
