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
        <li v-for="(link, i) in list" :key="i">
          <a href="#">{{ link.title }}</a>
          <img v-if="link.img" :src="link.img" alt="Logo Peppe" />
        </li>
      </ul>

      <ul>
        <li v-for="(link, i) in listRight" :key="i">
          <a class="d-flex" href="#" :class="link.icon ? 'fa fa-search' : ''">
            <img class="bg-white w-25" :src="link.img" alt="" />
            {{ link.title }}</a
          >
        </li>
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
  data() {
    return {
      list: [
        {
          title: "HOME",
          href: "#",
        },
        {
          title: "PAGES",
          href: "#",
        },
        {
          title: "MENU",
          href: "#",
        },
        {
          img: require("@/assets/img/h5-logo-divided-header.png"),
        },
        {
          title: "EVENT",
          href: "#",
        },
        {
          title: "BLOG",
          href: "#",
        },
        {
          title: "LANDING",
          href: "#",
        },
      ],

      listRight: [
        {
          img: require("@/assets/svg/svg-1.svg"),
          title: "CART",
        },
        {
          icon: "fa fa-search",
          title: "SEARCH",
        },
      ],
    };
  },
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

      &:hover {
        color: blue;
      }
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
