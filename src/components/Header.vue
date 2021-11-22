<template>
  <header class="header-container pb-5">
    <button class="button-left">PREV</button>
    <button class="button-right">NEXT</button>
    <!-- Inizio Navbar -->
    <div class="container d-flex justify-content-between align-items-center">
      <ul>
        <li><button class="header-button">ORDER ONLINE</button></li>
      </ul>

      <ul>
        <li><a href="#">HOME</a></li>
        <li><a href="#">PAGES</a></li>
        <li><a href="#">MENU</a></li>
        <li>
          <img
            src="@/assets/img/h5-logo-divided-header.png"
            alt="Logo Navbar"
          />
        </li>
        <li><a href="#">EVENT</a></li>
        <li><a href="#">BLOG</a></li>
        <li><a href="#">LANDING</a></li>
      </ul>

      <ul>
        <li><a href="#">CART</a></li>
        <li><a href="#">SEARCH</a></li>
      </ul>
    </div>
    <!-- Fine Navbar -->
    <!-- Inizio Hero -->
    <div class="container background-header-img">
      <img
        class="header-img-absolute"
        src="@/assets/img/h3-rev-img-6.png"
        alt=""
      />
    </div>
    <!-- Fine Hero -->
  </header>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style lang="scss">
@import "../style/variables";

.header-container {
  background-color: black;
  padding: $padding;
  position: relative;

  .header-button {
    background-color: orangered;
    border: none;
    padding: 10px 20px;
    color: $color_white;
  }

  ul {
    display: flex;
    list-style: none;

    li {
      display: flex;
      align-self: center;

      img {
        width: 140px;
      }
    }

    a {
      text-decoration: none;
      color: $color_white;
      padding: 0 20px;
    }
  }

  .background-header-img {
    background-image: url(../assets/img/h3-rev-img-5.png);
    text-align: center;
    background-position: center;
    background-repeat: no-repeat;
  }
}
</style>
