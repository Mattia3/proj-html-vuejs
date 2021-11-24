<template>
  <footer>
    <div class="row">
      <div class="col-6 d-flex background-black container-footer">
        <div class="col-3">
          <ul>
            <li class="title-oro pb-3"><h4>FIND OUR RESTAURANTS</h4></li>
            <li v-for="(element, i) in listFind" :key="i" class="pb-3">
              {{ element.indirizzo }} {{ element.città }} {{ element.numero }}
            </li>

            <li class="title-oro pt-5">
              Created with <i class="fa fa-heart-o" aria-hidden="true"></i> .by
              <span class="color-green">Qode interactive</span>
            </li>
          </ul>
        </div>
        <div class="col-5 d-flex justify-content-center">
          <ul>
            <li class="title-oro pb-3"><h4>WORKING HOURS</h4></li>
            <li v-for="(element, i) in listFooter" :key="i">
              <div class="title-oro">{{ element.title }}</div>
              <div
                :class="
                  element.subtitle === 'Kitchen Closed' ? 'title-orange' : ''
                "
                class="pb-3"
              >
                {{ element.subtitle }}
              </div>
            </li>

            <li class="title-oro">
              FOLLOW US:
              <span v-for="(icon, i) in listSocial" :key="i" class="text-white"
                ><i class="px-2" :class="icon.icon" aria-hidden="true"></i
              ></span>
            </li>
          </ul>
        </div>

        <div class="col-4 text-white">
          <h4>
            THE DON PEPPE CREW FIRST AND FOREMOST VALUES AN AUTHENTIC, WELL
            BAKED SLICE OF PIZZA.
          </h4>
        </div>
      </div>

      <div class="col-6 p-0">
        <div>
          <img src="@/assets/img/footer-img-1.jpg" alt="immagine footer" />
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  data() {
    return {
      listFooter: [
        {
          title: "MONDAY",
          subtitle: "Kitchen Closed",
        },
        {
          title: "TUSEDAY UNTIL FRIDAY",
          subtitle: "9:00 - 22:00",
        },
        {
          title: "SATURDAY*",
          subtitle: "Saturday 11 am to midnight",
        },
        {
          title: "SUNDAY",
          subtitle: "9:00 - 22:00",
        },
      ],

      listSocial: [
        {
          icon: "fa fa-twitter",
        },
        {
          icon: "fa fa-facebook",
        },
        {
          icon: "fa fa fa-instagram",
        },
        {
          icon: "fa fa-linkedin",
        },
      ],

      listFind: [
        {
          indirizzo: "1614 E. Bell Rd #104.",
          città: "Salerno, AZ 85022 ",
          numero: "(602)867-10010",
        },
        {
          indirizzo: "1614 E. Bell Rd #104.",
          città: "Salerno, AZ 85022 ",
          numero: "(602)867-10010",
        },
        {
          indirizzo: "1614 E. Bell Rd #104.",
          città: "Salerno, AZ 85022 ",
          numero: "(602)867-10010",
        },
        {
          indirizzo: "1614 E. Bell Rd #104.",
          città: "Salerno, AZ 85022 ",
          numero: "(602)867-10010",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
@import "../style/variables";

footer {
  color: lightgray;
  .container-footer {
    padding: 120px 0;
  }
  ul {
    list-style: none;
  }
}
</style>
