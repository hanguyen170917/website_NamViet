<template>
  <div class="header_nav">
    <header class="header">
      <div class="container">
        <div class="logo">
          <a href="#">
            <img src="../assets/logo2.png" alt="logo2" />
          </a>
        </div>
        <div class="contact">
          <img src="../assets/icon/phone-contact.png" alt="phone contact" />
          <span>Hotline: (028) 3 9320660 - 0903669949</span>
        </div>
        <div class="search">
          <input
            type="text"
            class="form-control"
            id="txtSearch"
            placeholder="Tìm kiếm ...."
          />
          <a href="#">
            <img src="../assets/icon/search.png" alt="iconSearch" />
          </a>
        </div>
        <div class="cart">
          <img src="../assets/icon/cart.png" alt="iconCart" />
        </div>
        <div class="acount">
          <img src="../assets/icon/user.png" alt="iconCart" />
        </div>
      </div>
    </header>
    <section class="menu">
      <div class="container" ref="navContent">
        <div class="toggler">
          <button class="btnToggle" @click="toggleMenu(1)">
            <img src="../assets/icon/menu/toggle.png" alt="iconToggle" />
          </button>
        </div>
        <ul class="nav_content">
          <!-- <li>
            <div class="toggler">
              <button class="btnToggle" @click="toggleMenu(1)">
                <img src="../assets/icon/menu/toggle.png" alt="iconToggle" />
              </button>
            </div>
          </li> -->
          <li>
            <div
              class="nav_item item1"
              style="margin-left: 32px"
              @click="toggleMenu(1)"
            >
              <img src="../assets/icon/menu/phone.png" alt="iconWatch" />
              <span>ĐIỆN THOẠI</span>
              <img src="../assets/icon/menu/chev_down.png" alt="iconChevDown" />
            </div>
          </li>
          <li>
            <div class="nav_item item1" @click="toggleMenu(2)">
              <img src="../assets/icon/menu/tablet.png" alt="iconWatch" />
              <span>MÁY TÍNH BẢNG</span>
              <img src="../assets/icon/menu/chev_down.png" alt="iconChevDown" />
            </div>
          </li>
          <li>
            <div class="nav_item item1" @click="toggleMenu(3)">
              <img src="../assets/icon/menu/watch.png" alt="iconWatch" />
              <span>WATCH</span>
              <img src="../assets/icon/menu/chev_down.png" alt="iconChevDown" />
            </div>
          </li>
          <li>
            <div class="nav_item item1" @click="toggleMenu(4)">
              <img src="../assets/icon/menu/laptop.png" alt="iconWatch" />
              <span>MÁY TÍNH APPLE</span>
              <img src="../assets/icon/menu/chev_down.png" alt="iconChevDown" />
            </div>
          </li>
          <li>
            <div class="nav_item item1" @click="toggleMenu(5)">
              <img src="../assets/icon/menu/sound.png" alt="iconWatch" />
              <span>LOA DI ĐỘNG</span>
              <img src="../assets/icon/menu/chev_down.png" alt="iconChevDown" />
            </div>
          </li>
          <li>
            <div class="nav_item item1" @click="toggleMenu(6)">
              <img src="../assets/icon/menu/sound.png" alt="iconWatch" />
              <span>TAI NGHE</span>
              <img src="../assets/icon/menu/chev_down.png" alt="iconChevDown" />
            </div>
          </li>
        </ul>
      </div>
    </section>
  </div>
  <div id="menu__dropdown" class="container" ref="menuDropdown">
    <div class="menu_dropdown" v-if="isShowMenu">
      <div class="row">
        <div class="col-lg-3 nav_left_custom">
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
        <div class="col-lg-9">
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

            <div class="quick_search">
              <div class="row">
                <QuickSearchItem />
                <QuickSearchItem />
                <QuickSearchItem />
                <QuickSearchItem />
                <QuickSearchItem />
                <QuickSearchItem />
                <QuickSearchItem />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import { ref, onBeforeUnmount, onMounted } from "vue";

import BrandItem from "./Brand.vue";
import QuickSearchItem from "./QuickSearch.vue";

export default {
  name: "dHeader",
  components: {
    BrandItem,
    QuickSearchItem,
  },
  setup() {
    const isShowMenu = ref(false);
    const activeMenu = ref(1);
    const navContent = ref(null);
    const menuDropdown = ref(null);

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
    return {
      isShowMenu,
      toggleMenu,
      activeMenu,
      navContent,
      menuDropdown,
    };
  },
};
</script>

<style></style>
