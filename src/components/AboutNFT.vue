<template>
  <div class="aboutNFT">
    <div class="container">
      <div class="row">
        <div class="col-12 col-lg-4">
          <div class="text firstText">
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
          </div>
        </div>
        <div class="col-12 col-lg-4">
          <div class="text">
            <div class="iconTitle">
              <img :src="img" alt="" />
              <p class="name">Fast Transaction</p>
            </div>
            <p class="description">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptate
              ex distinctio eligendi dolor non recusandae, facere dignissimos
              quas sunt rerum doloremque laudantium dolore quam
            </p>
          </div>
        </div>
        <div class="col-12 col-lg-4">
          <div class="text">
            <div class="iconTitle">
              <img :src="img1" alt="" />
              <p class="name">Growth Transaction</p>
            </div>
            <p class="description">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptate
              ex distinctio eligendi dolor non recusandae, facere dignissimos
              quas sunt rerum doloremque laudantium dolore quam
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SingularityTestAboutNFT",

  data() {
    return {
      img: "https://i.ibb.co/gW5b77T/card-tick-1-1.png",
      img1: "https://i.ibb.co/BT1gZqD/chart-square-2.png",
    };
  },

  mounted() {},

  methods: {},
};
</script>

<style>
.aboutNFT {
  min-height: 300px;
  background: rgba(217, 224, 236, 0.2);
  margin-bottom: 50px;
}
.aboutNFT .text {
  margin-top: 100px;
}
.aboutNFT .text .description {
  margin-left: 40px;
  font-family: "DM Sans";
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  color: #696969;
}
.aboutNFT .text .iconTitle {
  display: flex;
  align-items: center;
}
.aboutNFT .text .iconTitle img {
  height: 30px;
  margin-right: 10px;
}
.aboutNFT .text .iconTitle .name {
  font-family: 'DM Sans';
font-style: normal;
font-weight: 700;
font-size: 20px;
color: #000000;
}
.aboutNFT .text p {
  margin: 0;
  padding: 0;
}
.aboutNFT .firstText {
  font-family: "Integral CF";
  font-style: normal;
  font-weight: 700;
  font-size: 28px;
  color: #000000;
}
</style>