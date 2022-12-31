<template>
  <div class="topCollection">
    <div class="container">
      <div class="row">
        <div class="col-12 col-lg-4">
          <div class="firstCol">
            <div class="mainImage">
              <img :src="img" alt="" />
            </div>
            <div class="firstColFooter">
              <div class="footerContents">
                <p>
                  <img class="footerImage" :src="img3" alt="" />
                </p>
                <div>
                  <p>Thie Futr Abstr</p>
                  <p>10 in the stock</p>
                </div>
              </div>
              <div>
                <p>Highest Bid</p>
                <p class="footerIcon">
                  <img :src="icon1" alt="" />
                  0.25 ETH
                </p>
              </div>
            </div>
          </div>
        </div>
        <div class="col-12 col-lg-4">
          <div v-for="image in images" :key="image.id" class="secondCol">
            <div class="mainImage">
              <img :src="image.img" alt="" />
            </div>
            <div>
              <p class="title">The Futr Abstr</p>
              <div class="secondColDetails">
                <img :src="img3" alt="" />
                <p class="count">0.25 ETH</p>
                <p>1 of 8</p>
              </div>
              <div class="secondColButton">
                <button 
                :class="[image.isActive ?
                 'topCollection secondCol .secondColButton firstButton': 
                 'topCollection secondCol secondColButton featureButton']">Place a bid</button>
              </div>
            </div>
          </div>
        </div>
        <div class="col-12 col-lg-4">
          <div class="thirdCol">
            <div class="head">
              <p class="title">Top Collections Over</p>
              <p class="name">Last 7 days</p>
            </div>
            <div
              v-for="collection in topCollections"
              :key="collection.id"
              class="topProduct"
            >
              <p class="number">{{ collection.id }}</p>
              <div class="images">
                <img class="first" :src="collection.img" alt="" />
                <img class="second" :src="icon" alt="" />
              </div>
              <div class="mid">
                <p class="name">{{ collection.name }}</p>
                <p class="count">
                  <img :src="icon1" alt="" />
                  19,769.39
                </p>
              </div>
              <div>
                <p :class="[collection.isActive ? 'percentage': 'percentage2']">+{{ collection.percentage }}</p>
              </div>
              <hr>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SingularityTestTopCollection",

  data() {
    return {
      img: "https://i.ibb.co/g9txqbC/image-1-3.png",
      img1: "https://i.ibb.co/GFFbLJ7/image-1-1.png",
      img2: "https://i.ibb.co/4Tw9wJy/image-1-2.png",
      img3: "https://i.ibb.co/m9dP8mz/Group-105.png",
      icon: "https://i.ibb.co/K7j0v9x/verify-1.png",
      icon1: "https://i.ibb.co/h819ydL/ethereum-1.png",
      images: [
        { img: "https://i.ibb.co/b1Kbqhh/unsplash-p-Vo-EPp-Lw818-1.png",id:1,isActive:true },
        { img: "https://i.ibb.co/GFFbLJ7/image-1-1.png",id:2,isActive:false },
        { img: "https://i.ibb.co/dtKtdJ2/unsplash-Lpby-DENb-QQg-1.png",id:3,isActive:false },
      ],
      topCollections: [
        {
          img: "https://i.ibb.co/CPZwNNT/unsplash-5-MTf9-Xy-VVg-M.png",
          id: 1,
          name: "CryptoFunks",
          count: 19769.39,
          percentage: 26.52,isActive:false
        },
        {
          img: "https://i.ibb.co/kJ30Bz6/unsplash-f-T49-Qn-Fuc-Q8.png",
          id: 2,
          name: "Cryptix",
          count: 2769.39,
          percentage: 10.52,isActive:true
        },
        {
          img: "https://i.ibb.co/n7Cv0R7/unsplash-Wj-IB-6-Ux-A5-Q.png",
          id: 3,
          name: "Frensware",
          count: 9232.39,
          percentage: 2.52,isActive:true
        },
        {
          img: "https://i.ibb.co/V3Zq0Wf/unsplash-zk-NT5mik-Uuo.png",
          id: 4,
          name: "PunkArt",
          count: 3769.39,
          percentage: 1.52,isActive:true
        },
        {
          img: "https://i.ibb.co/kJ30Bz6/unsplash-f-T49-Qn-Fuc-Q8.png",
          id: 5,
          name: "Art Crypto",
          count: 10769.39,
          percentage: 2.52,isActive:false
        },
      ],
    };
  },

  mounted() {},

  methods: {},
};
</script>

<style>
.topCollection {
  margin-bottom: 50px;
}
.topCollection .firstColFooter,
.topCollection .footerContents,
.topCollection .secondCol,
.topCollection .secondColDetails,
.topCollection .thirdCol .topProduct {
  display: flex;
  align-items: center;
}
.topCollection .firstColFooter {
  margin-top: 10px;
  justify-content: space-between;
}
.topCollection .firstColFooter .footerImage {
  height: 30px;
  width: 30px;
  border-radius: 50%;
}
.topCollection .firstColFooter p,
.topCollection .secondCol p,
.topCollection .thirdCol p {
  margin: 0;
  padding: 0;
}
.topCollection .firstCol .mainImage img {
  width: 100%;
  height: 380px;
}
.topCollection .firstColFooter .footerIcon img {
  margin-top: -5px;
  height: 15px;
}
.topCollection .secondCol {
  margin-bottom: 20px;
}
.topCollection .secondColDetails img {
  height: 35px;
  width: 35px;
  border-radius: 50%;
}
.topCollection .secondCol .mainImage img {
  width: 145px;
  margin-right: 15px;
}
.topCollection .secondCol .title {
  font-family: "DM Sans";
  font-style: normal;
  font-weight: 700;
  font-size: 20px;
  color: #000000;
}
.topCollection .secondCol .secondColDetails {
  margin-top: 10px;
  justify-content: space-between;
}
.topCollection .secondColDetails .count {
  border: 1px solid #00ac4f;
  border-radius: 6px;
  color: #00ac4f;
  padding: 2px;
  margin-left: 5px;
  margin-right: 5px;
}
.topCollection .secondCol .secondColButton .featureButton {
  margin-top: 10px;
  width: 113px;
  height: 40px;
  padding: 15px;
  border: 1px solid #3d00b7;
  border-radius: 50px;
  color: #3d00b7;
}
.topCollection .secondCol .secondColButton .firstButton {
  margin-top: 10px;
  width: 113px;
  height: 40px;
  padding: 15px;
  background: #3d00b7;
  border-radius: 50px;
  border: none;
  color: white;
}
.topCollection .thirdCol .title {
  font-family: "Integral CF";
  font-style: normal;
  font-weight: 700;
  font-size: 20px;
  color: #000000;
}
.topCollection .thirdCol .head .name {
  font-family: "DM Sans";
  font-style: normal;
  font-weight: 700;
  font-size: 18px;
  color: #3d00b7;
}
.topCollection .thirdCol .topProduct {
  margin-top: 25px;
  justify-content: space-between;
  align-items: center;
}
.topCollection .thirdCol .topProduct .first {
  height: 50px;
  width: 50px;
  border-radius: 50%;
}
.topCollection .thirdCol .topProduct .images {
  position: relative;
}
.topCollection .thirdCol .topProduct .images .second {
  height: 30px;
  position: absolute;
  left: 26px;
  bottom: 25px;
}
.topCollection .thirdCol .topProduct .number {
  font-family: "DM Sans";
  font-style: normal;
  font-weight: 700;
  font-size: 24px;
  line-height: 103%;
  text-align: center;
  color: #000000;
}
.topCollection .thirdCol .topProduct .mid .name {
  font-family: "DM Sans";
  font-style: normal;
  font-weight: 500;
  font-size: 16px;
  letter-spacing: -0.025em;
  color: #000000;
}
.topCollection .thirdCol .topProduct .mid .count {
  display: flex;
  align-items: center;
  font-family: "Poppins";
  font-style: normal;
  font-weight: 600;
  font-size: 14px;
  letter-spacing: -0.025em;
  color: #636363;
}
.topCollection .thirdCol .topProduct .mid .count img {
  height: 15px;
  margin-right: 5px;
}
.topCollection .thirdCol .topProduct .percentage {
  font-family: "Poppins";
  font-style: normal;
  font-weight: 600;
  font-size: 20px;
  text-align: right;
  letter-spacing: -0.025em;
  color: #14c8b0;
}
.percentage2{
   font-family: "Poppins";
  font-style: normal;
  font-weight: 600;
  font-size: 20px;
  text-align: right;
  letter-spacing: -0.025em;
  color: red;
}
</style>