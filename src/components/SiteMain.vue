<template>
  <main id="site_main">
    <div class="hero_img"></div>
    <section class="content_section container">
      <div class="section_title">
        <h2>CURRENT SERIES</h2>
      </div>
      <div class="row comic space_evenly">
        <Comics
          v-for="comic in comics"
          :key="comic.series"
          :image="comic.thumb"
          :series="comic.series"
          class="col-3"
        />
      </div>
    </section>
    <!-- /.content_section -->
    <section class="content_index">
      <ul class="index_options d-flex container">
        <li>
          <a href="#">
            <div class="index_link">
              <img src="../assets/img/buy-comics-digital-comics.png" alt="" />
              <h5>DIGITAL COMICS</h5>
            </div>
          </a>
        </li>
        <li>
          <a href="#">
            <div class="index_link">
              <img src="../assets/img/buy-comics-merchandise.png" alt="" />

              <h5>DC MERCHANDISE</h5>
            </div>
          </a>
        </li>
        <li>
          <a href="#">
            <div class="index_link">
              <img src="../assets/img/buy-comics-subscriptions.png" alt="" />

              <h5>SUBSCRIPTION</h5>
            </div>
          </a>
        </li>
        <li>
          <a href="#">
            <div class="index_link">
              <img
                src="../assets/img/buy-comics-shop-locator.png"
                alt=""
                class="locator_logo"
              />

              <h5>COMIC SHOP LOCATOR</h5>
            </div>
          </a>
        </li>
        <li>
          <a href="#">
            <div class="index_link">
              <img src="../assets/img/buy-dc-power-visa.svg" alt="" />

              <h5>DC POWER VISA</h5>
            </div>
          </a>
        </li>
      </ul>
    </section>
    <!-- /.content_index -->
  </main>
</template>

<script>
import Comics from "./Comics.vue";
export default {
  data() {
    return {
      comics: [
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
  components: {
    Comics,
  },
};
</script>

<style lang="scss">
@import "../assets/scss/variables.scss";
#site_main {
  background-color: $content_bg_color;

  .hero_img {
    height: 400px;
    background-image: url(../assets/img/jumbotron.jpg);
  }
  .content_section {
    color: $text_primary_color;
    padding: 3rem 0px;

    .section_title {
      width: 245px;
      background-color: $highlight_primary_color;
      margin-top: -4.5rem;
      margin-bottom: 1rem;
      h2 {
        padding: 0.5rem 1rem;
      }
    }
  }

  .content_index {
    background-color: $highlight_primary_color;
    padding: 3rem 0px;

    .index_options {
      justify-content: space-around;
      align-items: center;

      h5 {
        color: $text_primary_color;
        font-weight: normal;
        padding-left: 10px;
      }
    }

    .index_link {
      display: flex;
      align-items: center;
    }

    .locator_logo {
      width: 30px;
    }

    img {
      width: 40px;
    }
  }
}
</style>