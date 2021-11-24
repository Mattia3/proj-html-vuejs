<template>
  <div class="row row-cols-6 text-center pb-5">
    <div v-for="(card, i) in listPizza" :key="i" class="col position-relative">
      <img class="img-pizze" :src="card.img" alt="PIZZA BISMARK" />
      <h6 class="title-oro fw-bold pt-3">{{ card.title }}</h6>
      <span v-if="card.muted" class="text-muted text-decoration-line-through"
        >$5.00</span
      >
      <span class="title-orange px-2">{{ card.price }}</span>
      <p v-if="card.sold" class="soldout-pizza">SOLD</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardPizza",
  data() {
    return {
      listPizza: [
        {
          img: require("@/assets/img/h3-product-img-1a-100x100.png"),
          title: "BISMARK",
          price: "$30.00",
          muted: true,
        },
        {
          img: require("@/assets/img/h3-product-img-2a-150x150.png"),
          title: "FIORI DI ZUCCA",
          price: "$7.00 - $50.00",
        },
        {
          img: require("@/assets/img/h3-product-img-6a-100x100.png"),
          title: "VALDOSTANA",
          price: "$55.00",
          sold: true,
        },
        {
          img: require("@/assets/img/h3-product-img-4a-150x150.png"),
          title: "PIZZA TARTUFATA",
          price: "$45.00",
        },
        {
          img: require("@/assets/img/h3-product-img-5a-150x150.png"),
          title: "FRANCESCANA",
          price: "$25.00",
        },
        {
          img: require("@/assets/img/h3-product-img-3a-150x150.png"),
          title: "CAMPAGNOLA",
          price: "$50 - $95.00",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "../style/variables";

.img-pizze {
  width: 70%;
}

.soldout-pizza {
  position: absolute;
  right: 63px;
  top: 14px;
  background: $color_text;
  border-radius: 50%;
  width: 60px;
  height: 60px;
  color: $color_white;
  line-height: 60px;
}
</style>
