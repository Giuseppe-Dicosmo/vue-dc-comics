<template>
  <section class="container-Content">
    <span class="Content-jumbotron"></span>
    <div class="container">
      <button class="button-series">Content series</button>
      <div class="ciao">
        <ul>
          <fumettiShop
            v-for="(anteprima, i) in fumetti"
            :key="i"
            :src="anteprima.thumb"
            :title="anteprima.series"
          />
        </ul>
      </div>
      <button class="button-more">load more</button>
    </div>
  </section>
</template>

<script>
import fumettiShop from "./fumettiShop.vue";
export default {
  name: "MainContent",
  components: {
    fumettiShop,
  },
  data() {
    return {
      fumetti: [
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
          price: "$19.99",
          series: "Action Comics",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
          price: "$3.99",
          series: "American Vampire 1976",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
          price: "$16.99",
          series: "Aquaman",
          type: "graphic novel",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
          price: "$2.99",
          series: "Batgirl",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$3.99",
          series: "Batman",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          price: "$2.99",
          series: "Batman Beyond",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
          price: "$3.99",
          series: "Batman/Superman",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
          price: "$4.99",
          series: "Batman/Superman Annual",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
          price: "$5.99",
          series: "Batman: The Joker War Zone",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
          price: "$6.99",
          series: "Batman: Three Jokers",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
          price: "$4.99",
          series: "Batman: White Knight Presents: Harley Quinn",
          type: "comic book",
        },
        {
          thumb:
            "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
          price: "$16.99",
          series: "Catwoman",
          type: "graphic novel",
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
$brand_color: white;
$brand_blue: #0282f9;

.container-Content {
  height: 150vh;
  width: 100%;
  background-color: black;
  color: $brand_color;
  display: flex;
  flex-direction: column;
  align-items: center;

  .Content-jumbotron {
    background: url("../assets/jumbotron.jpg") no-repeat top center;
    background-size: cover;
    width: 100%;
    height: 40%;
  }

  .container {
    width: 100%;
    height: 100%;
    position: relative;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    .button-series {
      border: 1px solid $brand_blue;
      background: $brand_blue;
      color: $brand_color;
      text-transform: uppercase;
      font-size: 20px;
      padding: 10px;
      cursor: pointer;
      position: absolute;
      bottom: 100%;
      left: 0;
      transform: translate(0, 50%);
    }

    .ciao {
      height: 100%;
      display: flex;
      justify-content: center;
      align-items: center;

      ul {
        width: 95%;
        height: 80%;
        display: flex;
        flex-flow: row wrap;
        gap: 20px;
        list-style-type: none;
      }
    }
  }

  .button-more {
    border: 1px solid $brand_blue;
    background: $brand_blue;
    color: $brand_color;
    text-transform: uppercase;
    font-size: 13px;
    padding: 10px 35px;
    margin-bottom: 20px;
    cursor: pointer;
  }
}
</style>
