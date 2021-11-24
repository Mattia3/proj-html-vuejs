<template>
  <div class="row-cols-4 d-flex">
    <div class="col position-relative" v-for="(card, i) in listCard" :key="i">
      <img class="main-img-section" :src="card.img" alt="" />
      <div class="overlay">
        <i class="fa fa-eye icon-hover" aria-hidden="true"></i>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Card",
  data() {
    return {
      listCard: [
        {
          img: require("@/assets/img/h3-img-1.jpg"),
        },
        {
          img: require("@/assets/img/h3-img-2.jpg"),
        },
        {
          img: require("@/assets/img/h3-img-3.jpg"),
        },
        {
          img: require("@/assets/img/h3-img-4.jpg"),
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "../style/variables";

.main-img-section {
  width: 100%;
  border: 7px solid $color_white;
}

.overlay {
  position: absolute;
  bottom: 100%;
  left: 0;
  right: 0;
  background-color: white;
  overflow: hidden;
  width: 100%;
  height: 0;
  transition: 0.5s ease;
}

.col:hover .overlay {
  bottom: 0;
  height: 100%;
}

.icon-hover {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  text-align: center;
  font-size: 30px;
  background: $color_text;
  padding: 28px;
  border-radius: 50%;
  color: white;
}
</style>
