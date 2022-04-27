<template>
  <div class="header_nav">
    <header>
      <div class="header">
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

    <section class="content menu">
      <ul class="nav_content">
        <li>
          <div class="toggler">
            <button class="btnToggle">
              <img src="../assets/icon/menu/toggle.png" alt="iconToggle" />
            </button>
          </div>
        </li>
        <li>
          <div class="nav_item item1" style="margin-left: 32px">
            <img src="../assets/icon/menu/phone.png" alt="iconPhone" />
            <span>ĐIỆN THOẠI</span>
            <img src="../assets/icon/menu/chev_down.png" alt="iconChevDown" />
          </div>
        </li>
        <li>
          <div class="nav_item item1 item2">
            <img src="../assets/icon/menu/tablet.png" alt="iconTablet" />
            <span>MÁY TÍNH BẢNG</span>
            <img src="../assets/icon/menu/chev_down.png" alt="iconChevDown" />
          </div>
        </li>
        <li>
          <div class="nav_item item1 item3">
            <img src="../assets/icon/menu/watch.png" alt="iconWatch" />
            <span>WATCH</span>
            <img src="../assets/icon/menu/chev_down.png" alt="iconChevDown" />
          </div>
        </li>
        <li>
          <div class="nav_item item1 item4">
            <img src="../assets/icon/menu/laptop.png" alt="iconLaptop" />
            <span>MÁY TÍNH APPLE</span>
            <img src="../assets/icon/menu/chev_down.png" alt="iconChevDown" />
          </div>
        </li>
        <li>
          <div class="nav_item item1 item5">
            <img src="../assets/icon/menu/sound.png" alt="iconSound" />
            <span>LOA DI ĐỘNG</span>
            <img src="../assets/icon/menu/chev_down.png" alt="iconChevDown" />
          </div>
        </li>
        <li>
          <div class="nav_item item1 item6">
            <img src="../assets/icon/menu/sound.png" alt="iconSound" />
            <span>TAI NGHE</span>
            <img src="../assets/icon/menu/chev_down.png" alt="iconChevDown" />
          </div>
        </li>
      </ul>
    </section>
  </div>
</template>

<script>
export default {
  name: "dHeader",
};
</script>

<style></style>
