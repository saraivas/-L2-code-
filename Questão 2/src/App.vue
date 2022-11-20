<template>
  <div class="all-content">
    <topBar />

    <HeaderPage />
    <p>Latest live auction</p>
    <div class="carousel" v-dragscroll.x="true">
      <div class="item-carousel" v-for="item in itemsList" :key="item.id">
        <img src="./assets/images/Image3.png" alt="" />
        <div class="title-price">
          <h6>{{ item.title }}</h6>
          <p class="price">{{ item.price }}</p>
        </div>
        <div class="time">
          <img src="./assets/images/Vector.png" alt="" />
          <p>{{ item.time }}</p>
        </div>
        <div class="divider"></div>
        <div class="peoples">
          <div class="photos">
            <img src="./assets/icons/01.png" alt="" />
            <img src="./assets/icons/01.png" alt="" />
            <img src="./assets/icons/01.png" alt="" />
            <img src="./assets/icons/01.png" alt="" />
          </div>
          <div class="text">
            <p>{{ item.people }}</p>
            <div class="likes">
              <img src="./assets/icons/Vector.png" alt="" />{{ item.like }}
            </div>
          </div>
        </div>
      </div>

      <div class="arrow-slide">
        <img src="./assets/icons/arrow.png" alt="" />
      </div>
    </div>

    <div class="central-content">
      <imageText />
      <div class="divider"></div>
      <sectionIcons />
      <footerPage />
    </div>
  </div>
</template>

<script>
//import VueAIcarousel from "vue-ai-carousel";
import HeaderPage from "./components/HeaderPage.vue";
import footerPage from "./components/footerPage.vue";
import topBar from "./components/topBar.vue";
import imageText from "./components/imageText.vue";
import sectionIcons from "./components/sectionIcons.vue";

import { dragscroll } from "vue-dragscroll";

export default {
  name: "App",
  components: {
    //VueAIcarousel,
    HeaderPage,
    footerPage,
    topBar,
    imageText,
    sectionIcons,
  },
  directives: {
    dragscroll: dragscroll,
  },
  data() {
    return {
      itemsList: [
        {
          id: 1,
          url: "./assets/images/Image1.png",
          title: "Tristique diam a, enim, eros tellus. Viverra etiam",
          price: "2.55 ETH",
          time: "2:41 min left",
          people: "35 people are bidding",
          like: "120",
        },
        {
          id: 2,
          url: "./assets/images/Image.png",
          title: "Vulputate felis purus viverra morbi facilisi eget",
          price: "3.19 ETH",
          time: "57:15 min left",
          people: "35 people are bidding",
          like: "120",
        },
        {
          id: 3,
          url: "./assets/images/Image3.png",
          title: "Dui accumsan leo vestibulum ornare eu",
          price: "1.11 ETH",
          time: "22:59 min left",
          people: "35 people are bidding",
          like: "120",
        },
        {
          id: 4,
          url: "./assets/images/Image4.png",
          title: "Senectus adipiscing nascetur accumsan etiam",
          price: "1.63 ETH",
          time: "37:01 min left",
          people: "35 people are bidding",
          like: "120",
        },
        {
          id: 5,
          url: "./assets/images/Image5.png",
          title: "Mattis at diam lorem nisl nam sed sociis",
          price: "2.55 ETH",
          time: "12:15 min left",
          people: "35 people are bidding",
          like: "120",
        },
      ],
    };
  },
  props: {
    item: {},
  },
  mounted() {},
};
</script>

<style lang="less">
* {
  background: #060714;
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Sora", sans-serif;
}
html {
  width: 100vw;
}
#app {
  width: 100%;
  margin: 0;
  padding: 0;
}

.all-content {
  width: 100%;
  p {
    font-style: normal;
    font-weight: 600;
    font-size: 36px;
    line-height: 45px;
    text-align: center;
    letter-spacing: 0.2px;
    color: #ffffff;
    margin: 50px;
  }
}

.carousel {
  display: flex;
  gap: 24px;
  overflow: auto;
  overflow: hidden;
  scroll-margin-right: 65px;

  &:hover {
    cursor: e-resize;
  }
  .item-carousel {
    width: 448px;
    height: 767px;
    border: 1px solid #262840;
    border-radius: 20px;
    padding: 24px 24px 0 24px;
    margin-bottom: 135px;

    p {
      margin: 0;
    }

    img {
      width: 400px;
      height: 520px;
      border-radius: 20px;
      object-fit: cover;
      margin-bottom: 24px;
    }

    .title-price {
      display: flex;
      align-items: center;
      justify-content: space-between;
      margin-bottom: 24px;

      h6 {
        font-weight: 600;
        font-size: 20px;
        color: #ffffff;
        width: 266px;
        height: 50px;

        text-align: left;
      }

      .price {
        padding: 8px 14px;
        width: 99px;
        height: 36px;
        background: rgba(81, 76, 255, 0.15);
        border-radius: 4px;
        color: #514cff;
        font-size: 16px;
        font-weight: 600;
        line-height: 20px;
        letter-spacing: 0.2px;
      }
    }

    .time {
      width: 112px;
      height: 21px;
      display: flex;
      align-items: center;
      margin-bottom: 28px;

      img {
        width: 14.22px;
        height: 16px;
        margin: 0;
        margin-right: 11.28px;
      }
      p {
        font-family: "Inter", sans-serif;
        font-weight: 400;
        font-size: 13px;
        letter-spacing: 0.2px;
        color: #ffffff;
      }
    }

    .divider {
      border: 1px solid #262840;
      margin-bottom: 20px;
    }
    .peoples {
      display: flex;
      align-items: center;
      width: 293px;
      height: 32px;

      .photos {
        display: flex;
        width: 128px;
        height: 32px;
        margin-right: 16px;
        img {
          margin: 0;
          width: 32px;
          height: 32px;
        }
      }

      .text {
        display: flex;
        align-items: center;
        justify-content: space-between;

        p {
          margin: 0;
          font-weight: 400;
          font-size: 14px;
          color: #7780a1;
          width: 149px;
          letter-spacing: 0;
        }
        .likes {
          display: flex;
          align-items: center;
          justify-content: space-between;
          margin-left: 54px;
          font-size: 14px;
          img {
            margin: 0;
            width: 16.67px;
            height: 14.86px;
            margin-right: 9.67px;
          }
          color: #7780a1;
        }
      }
    }
  }

  position: relative;
  .arrow-slide {
    position: absolute;
    width: 120px;
    height: 120px;
    background: rgba(38, 40, 64, 0.8);
    box-shadow: 0px 25px 75px rgb(6 7 20 / 10%);
    -webkit-backdrop-filter: blur(3.5px);
    backdrop-filter: blur(3.5px);
    border-radius: 79px;
    top: 230px;
    right: 135px;
    display: flex;
    justify-content: center;
    align-items: center;

    img {
      background: #06071400;
    }
  }
}

.central-content {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  .divider {
    width: 1392px;
    height: 0px;
    left: 264px;
    top: 2982px;
    border: 1px solid #7780a196;
    margin-bottom: 148px;
  }
}
</style>
