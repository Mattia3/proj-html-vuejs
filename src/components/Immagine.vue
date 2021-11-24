<template>
  <div>
    <div class="row">
      <div class="col-1 p-0">
        <div class="background-img-judge-1"></div>
      </div>
      <div class="col-10 p-0">
        <div class="background-img-judge"></div>
      </div>
      <div class="col-1 p-0">
        <div class="background-img-judge-3"></div>
      </div>
    </div>

    <div class="row">
      <div class="col-1 p-0">
        <div class="background-img-judge-4"></div>
      </div>
      <div class="col-10 p-0">
        <div class="background-img-judge-5">
          <div class="col-6 container-text">
            <h1 class="text-white fw-bold">
              GO AHEAD AND BUILD YOUR OWN PIZZA WE WON'T JUDGE!
            </h1>
          </div>
        </div>
      </div>
      <div class="col-1 p-0">
        <div class="background-img-judge-6 position-relative">
          <img
            class="svg-pizza-special-2"
            src="@/assets/svg/svg-4.svg"
            alt=""
          />
        </div>
      </div>
    </div>

    <div class="row">
      <div class="col-1 p-0">
        <div class="background-img-judge-7"></div>
      </div>
      <div class="col-10 p-0">
        <div class="background-img-judge-8"></div>
      </div>
      <div class="col-1 p-0">
        <div class="background-img-judge-9"></div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Immagine",
};
</script>

<style lang="scss">
@import "../style/variables";

.background-img-judge {
  background-image: url(../assets/img/h3-background-img.jpg);
  height: 100px;
  background-position: bottom;
  background-position-x: right;
}

.background-img-judge-3 {
  background-image: url(../assets/img/h3-background-img.jpg);
  height: 100px;
}

.background-img-judge-1 {
  background-image: url(../assets/img/h3-background-img.jpg);
  height: 100px;
  background-position-x: right;
  background-position-y: bottom;
}

.background-img-judge-4 {
  background-image: url(../assets/img/h3-background-img.jpg);
  height: 270px;
  background-position-x: right;
}

.background-img-judge-5 {
  background-image: url(../assets/img/h3-background-img.jpg);
  height: 270px;
  background-position-y: 7%;
  background-position-x: 40%;
}

.background-img-judge-6 {
  background-image: url(../assets/img/h3-background-img.jpg);
  height: 270px;
}

.background-img-judge-7 {
  background-image: url(../assets/img/h3-background-img.jpg);
  height: 100px;
  background-position-x: right;
  background-position-y: 70%;
}

.background-img-judge-8 {
  background-image: url(../assets/img/h3-background-img.jpg);
  height: 100px;
  background-position-x: right;
  background-position-y: 61%;
}

.background-img-judge-9 {
  background-image: url(../assets/img/h3-background-img.jpg);
  height: 100px;
  background-position-x: 20%;
  background-position-y: 20%;
}

.container-text {
  padding: 0px 333px;
  position: absolute;
}
.svg-pizza-special-2 {
  position: absolute;
  border-radius: 50%;
  background: rgba(246, 247, 242, 255);
  width: 40px;
  height: 40px;
  object-fit: none;
  left: 50%;
  bottom: 10%;
}
</style>
