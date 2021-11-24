<template>
  <main>
    <!-- Inizio prima section -->
    <Card></Card>
    <!-- Fine prima section -->

    <!-- Inizio Seconda Section -->
    <div class="background-image-hello">
      <button class="button-left">PREV</button>
      <button class="button-right">NEXT</button>

      <div class="container container-hello">
        <div class="row justify-content-center">
          <div class="col-9">
            <img src="@/assets/svg/svg-11.svg" alt="" />
            <h4 class="fw-bold">
              "FORGET THE TRENDY PIZZA SHOPS, THIS HIDDEN SPOT MAKES THE BEST
              NEW YORK-STYLE PIZZA SLICE IN NAPLES"
            </h4>
            <p class="text-color">WASHINGTON POST 2018</p>
            <div class="d-flex justify-content-center">
              <div class="next-slider"></div>
              <div class="next-slider mx-2"></div>
              <div class="next-slider"></div>
            </div>
          </div>
        </div>
      </div>
      <img class="pizza-svg" src="@/assets/svg/svg-4.svg" alt="" />
    </div>
    <!-- Fine Seconda Section -->

    <!-- Inizio Special Section -->
    <div class="row py-2">
      <div class="col-6">
        <img class="img-special" src="@/assets/img/h1-img-4.jpg" alt="" />
      </div>

      <div class="col-6 container-special position-relative">
        <div class="col-5">
          <h3 class="fw-bold">SPECIALS*</h3>
          <p>
            Lorem ipsum dolor sit amet, consectur adipiscing elit. Praesent ut.
          </p>
          <div class="d-flex">
            <h4 class="pe-3 text-danger fw-bold">$10</h4>
            <div>
              <h4 class="fw-bold">COMBO MEZZO</h4>
              <p>
                Lorem ipsum dolor sit amet, consectur adipiscing elit. Praesent
                ut.
              </p>
            </div>
          </div>
          <div class="d-flex">
            <h4 class="pe-3 text-danger fw-bold">$20</h4>
            <div>
              <h4 class="fw-bold">COMBO MEZZO</h4>
              <p>
                Lorem ipsum dolor sit amet, consectur adipiscing elit. Praesent
                ut.
              </p>
            </div>
          </div>
          <div class="d-flex">
            <h4 class="pe-3 text-danger fw-bold">$30</h4>
            <div>
              <h4 class="fw-bold">COMBO GRANDE</h4>
              <p>
                Lorem ipsum dolor sit amet, consectur adipiscing elit. Praesent
                ut.
              </p>
            </div>
          </div>
        </div>
        <img class="svg-pizza-special" src="@/assets/svg/svg-4.svg" alt="" />
      </div>
    </div>
    <!-- Fine Special Section -->

    <!-- Inizio judge section -->
    <Immagine></Immagine>
    <!-- Fine judge section -->

    <!-- Inizio section people -->
    <CardPeople></CardPeople>
    <!-- Fine section people -->

    <!-- Inizio section loghi -->
    <div class="row container-loghi">
      <div class="col-12 d-flex justify-content-center py-5">
        <img src="@/assets/img/h1-clients-img-4.png" alt="" />
        <img src="@/assets/img/h1-clients-img-3.png" alt="" />
        <img src="@/assets/img/h1-clients-img-1.png" alt="" />
        <img src="@/assets/img/h1-clients-img-2.png" alt="" />
        <img src="@/assets/img/h1-clients-img-5.png" alt="" />
      </div>
    </div>
    <!-- Fine section loghi -->
    <!-- Inzio pizze -->
    <div class="container py-5 text-center">
      <div class="row justify-content-center">
        <div class="col-6">
          <h6 class="text-danger">CHOSE YOUR FLAVOR</h6>
          <h2 class="fw-bold">THE BEST PIZZA MENU IN TOWN</h2>

          <p class="text-muted">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatem
            inventore et laboriosam? Beatae dolor asperiores aliquid, illum
          </p>
        </div>
      </div>
    </div>
    <CardPizza></CardPizza>

    <!-- Fine pizze -->
    <!-- Inizio section date -->
    <div class="row">
      <div
        class="
          col-6
          d-flex
          justify-content-center
          align-items-center
          text-white
          background-date
          p-0
        "
      >
        <div class="col-6">
          <h6 class="title-orange">MADE WITH LOVE</h6>
          <h3 class="pb-4">DELISH PIZZA DEALS</h3>
          <div class="d-flex text-date">
            <div class="pe-4">
              <h4 class="title-orange fs-1">02</h4>
              <h5>NOV</h5>
            </div>
            <div>
              <h3>TRADITIONAL NEAPOLTINA PIES IN KYOTO PIZZA MERCATO</h3>
              <p class="title-orange">204 E. Pizzetta Tommaso</p>
            </div>
          </div>
          <div class="d-flex text-date py-4">
            <div class="pe-4">
              <h3 class="title-orange fs-1">03</h3>
              <h5>NOV</h5>
            </div>
            <div>
              <h4>TERARAZZA PATIO DINING SPACE OPENING THIS WEEKEND</h4>
              <p class="title-orange">204 E. Pizzetta Tommaso</p>
            </div>
          </div>
          <div class="d-flex py-4">
            <div class="pe-4">
              <h4 class="title-orange fs-1">05</h4>
              <h5>NOV</h5>
            </div>
            <div>
              <h3>SIENNA PRIVATE DINING ROOM WITH STEPHANIE BRUUN</h3>
              <p class="title-orange">204 E. Pizzetta Tommaso</p>
            </div>
          </div>
        </div>
      </div>

      <div class="col-6 p-0">
        <img src="@/assets/img/h3-img-5a.jpg" alt="" />
      </div>
    </div>
    <!-- Fine section date -->
    <!-- Inizio input -->
    <div class="background-input-img">
      <div class="row-cols-12 row position-relative">
        <form class="form-input" action="">
          <input type="text" placeholder="1 Person" />
          <h6 class="text-white px-3">FOR</h6>
          <input type="text" placeholder="11/29/2020" />
          <h6 class="text-white px-3">AT</h6>
          <input class="me-5" type="text" placeholder="7:00 pm" />
          <button class="input-orange">BOOK A TABLE</button>
        </form>
        <h6 class="subtitle-form">*Powered by OpenTable</h6>
      </div>
    </div>
    <!-- Fine input -->
  </main>
</template>

<script>
import Card from "./Card.vue";
import CardPeople from "./CardPeople.vue";
import CardPizza from "./CardPizza.vue";
import Immagine from "./Immagine.vue";

export default {
  name: "Main",
  components: {
    Card,
    CardPeople,
    CardPizza,
    Immagine,
  },
};
</script>

<style lang="scss">
@import "../style/variables";

.background-image-hello {
  background-image: url(../assets/img/h3-testimonials-bckgrnd.jpg);
  background-position: center;
  position: relative;
  padding: $padding;

  .container-hello {
    padding: $padding_large;
    text-align: center;
  }

  .text-color {
    color: $color_text;
  }

  .pizza-svg {
    position: absolute;
    right: 70px;
    bottom: 30px;
  }
}

.container-special {
  display: flex;
  align-items: center;
  justify-content: center;

  .svg-pizza-special {
    position: absolute;
    right: 40px;
    bottom: 200px;
    border-radius: 50%;
    background: rgba(246, 247, 242, 255);
    width: 40px;
    height: 40px;
    object-fit: none;
  }
}

.img-special {
  width: 100%;
}

.container-loghi {
  background-color: rgba(247, 247, 242, 255);
}

.background-date {
  background-color: black;
  height: 800px;

  .text-date {
    border-bottom: 1px dotted;
  }
}

.background-input-img {
  background-image: url(../assets/img/h3-background-img-3.jpg);
  margin: 10px 0;
  .form-input {
    display: flex;
    justify-content: center;
    padding: $padding_large;
    align-items: center;

    input {
      padding: 10px;
      border: 2px solid black;
      font-size: small;
    }

    .input-orange {
      color: white;
      background-color: $color_text;
      color: white;
      padding: 10px 37px;
      border: none;
    }
  }
  .subtitle-form {
    bottom: 62px;
    position: absolute;
    left: 26%;
    color: white;
    font-size: small;
  }
}

.next-slider {
  width: 10px;
  height: 10px;
  border-radius: 50%;
  background: lightgray;
}
</style>
