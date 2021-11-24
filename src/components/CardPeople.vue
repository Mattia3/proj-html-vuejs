<template>
  <div class="row row-cols-4">
    <div
      v-for="(card, i) in ListCardPeople"
      :key="i"
      class="col p-0 position-relative"
    >
      <img class="img-people" :src="card.img" alt="" />
      <div class="overlay-2">
        <div class="overlay-text">
          <h1>FRANK BAILEY</h1>
          <p>kitchen porter</p>
          <p>
            <i class="fa fa-instagram" aria-hidden="true"></i
            ><i class="fa fa-twitter px-3" aria-hidden="true"></i>
            <i class="fa fa-facebook" aria-hidden="true"></i>
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CardPeople",
  data() {
    return {
      ListCardPeople: [
        {
          img: require("@/assets/img/h1-team-1a-700x700.jpg"),
        },
        {
          img: require("@/assets/img/h1-team-2a.jpg"),
        },
        {
          img: require("@/assets/img/h1-team-4a.jpg"),
        },
        {
          img: require("@/assets/img/h1-team-3a.jpg"),
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "../style/variables";

.img-people {
  width: 100%;
  padding: 10px 0;
}

.overlay-2 {
  position: absolute;
  bottom: 100%;
  left: 0;
  right: 0;
  background-color: white;
  overflow: hidden;
  width: 100%;
  height: 0;
  transition: 0.5s ease;
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  color: white;
}
.overlay-text {
  background: $color_text;
  padding: 162px 75px;
}

.col:hover .overlay-2 {
  bottom: 0;
  height: 100%;
}
</style>
