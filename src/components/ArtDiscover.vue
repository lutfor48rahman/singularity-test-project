<template>
  <div class="discoverArt">
    <div class="container">
      <div class="row">
        <div class="col-12 col-lg-8">
          <p class="name">
            Discover,And Collect Digital Art NFTS
          </p>
          <p class="description">
            Digital marketplace for crypto collectibles and non-fungible tokens (NFTs). Buy, Sell, and discover exclusive digital assets.
          </p>
          <div class="discoverButton">
            <button>Explore Now</button>
          </div>
          <div class="viewer">
            <div>
              <p class="countView">98K+</p>
              <p class="nameView">Artwork</p>
            </div>
            <div>
              <p class="countView">12K+</p>
              <p class="nameView">Actions</p>
            </div>
            <div>
              <p class="countView">15K+</p>
              <p class="nameView">Artists</p>
            </div>
          </div>
        </div>
        <div class="col-12 col-lg-4">
          <div class="mirrorImage">
            <div>
              <img class="image1" :src="img1" alt="" />
            <img class="image2" :src="img2" alt="" />
            <img class="image3" :src="img" alt="" />
              <img class="image4" :src="img3" alt="" />
            </div>
              <div class="imageContent">
                <p class="title">Abstr Gradient NFT</p>
                <div class="imageTitle">
                  <img :src="img4" alt="">
                  <p class="name">Arkhan17</p>
                </div>
              </div>
              <div class="timer">
                <div class="timeTitle">
                  <p class="timeHead">Current bid</p>
                  <p class="timeHead"><span>Ends in</span></p>
                </div>
                <div class="totalTime">
                  <p class="timeTable"> <img src="" alt=""> 0.25 ETH</p>
                  <p class="timeTable">12h 43m 42s</p>
                </div>
              </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SingularityTestArtDiscover",

  data() {
    return {
      img: "https://i.ibb.co/GFFbLJ7/image-1-1.png",
      img1: "https://i.ibb.co/4Tw9wJy/image-1-2.png",
      img2: "https://i.ibb.co/g9txqbC/image-1-3.png",
      img3:"https://i.ibb.co/x8fPSp7/Group-83.png",
      img4:"https://i.ibb.co/m9dP8mz/Group-105.png",
      images: [
        { img: "https://i.ibb.co/GFFbLJ7/image-1-1.png", id: 1 },
        { img: "https://i.ibb.co/4Tw9wJy/image-1-2.png", id: 2 },
        { img: "https://i.ibb.co/g9txqbC/image-1-3.png", id: 3 },
        { img: "https://i.ibb.co/nDvSp6G/image-1.png", id: 4 },
      ],
    };
  },

  mounted() {},

  methods: {},
};
</script>

<style>
.discoverArt {
  margin-top: 130px;
  margin-bottom: 80px;
}
.discoverArt .name {
  width: 612px;
  font-family: "Integral CF";
  font-style: normal;
  font-weight: 600;
  font-size: 35px;
  line-height: 48px;
  letter-spacing: 0.05em;
  text-transform: uppercase;
  color: #000000;
}
.discoverArt .description {
  width: 471px;
  font-family: "DM Sans";
  font-style: normal;
  font-weight: 400;
  font-size: 20px;
  color: #565656;
}
.discoverArt .discoverButton {
  margin-top: 50px;
}
.discoverArt .discoverButton button {
  width: 170px;
  height: 55px;
  background: #3d00b7;
  border-radius: 60px;
  border: none;
  color: white;
  transition: 0.4s;
}
.discoverArt .discoverButton button:hover {
  background: #7f48ee;
  font-weight: bold;
  color: white;
}
.viewer {
  margin-top: 20px;
  width: 60%;
  display: flex;
  justify-content: space-between;
}
.viewer p {
  margin: 0;
  padding: 0;
}
.viewer .countView {
  font-family: "Integral CF";
  font-style: normal;
  font-weight: 700;
  font-size: 40px;
  letter-spacing: 0.05em;
  color: #000000;
}
.viewer .nameView {
  font-family: "DM Sans";
  font-style: normal;
  font-weight: 400;
  font-size: 20px;
  color: #565656;
}
.mirrorImage {
    align-items: center;
  position: relative;
}
.discoverArt .mirrorImage {
  margin-top: 50px;
  position: relative;
}
.mirrorImage .image1 {
  height: 220px;
}
.mirrorImage .image2 {
  height: 245px;
  position: absolute;
  left: -14%;
  bottom: -16px;
}
.mirrorImage .image3 {
  height: 280px;
  position: absolute;
  left: -32%;
  bottom: -34px;
}
.mirrorImage .image4 {
  height: 90px;
 position: absolute;
 right: 425px;
 bottom: 45px;
}
.mirrorImage .imageContent p,
.mirrorImage .timer .timeTitle p,
.mirrorImage .timer .totalTime p{
 margin: 0;
}
.mirrorImage .imageContent {
 position: absolute;
 top:0px;
 left:-90px;
}
.mirrorImage .imageContent .title{
  font-family: 'DM Sans';
  font-style: normal;
  font-weight: 700;
  font-size: 22px;
  letter-spacing: -0.05em;
  color: #FFFFFF;
}
.mirrorImage .imageContent .imageTitle{
  margin-top: -10px;
  display: flex;
  align-items: center;
}
.mirrorImage .imageContent .imageTitle img{
  height: 30px;
  margin-right: 5px;
}
.mirrorImage .imageContent .imageTitle .name {
  font-family: 'DM Sans';
  font-style: normal;
  font-weight: 700;
  font-size: 16px;
  color: white;
}
.mirrorImage .timer{
  width: 270px;
height: 63.85px;
  color: white;
  background: rgba(255, 255, 255, 0.2);
  border-radius: 12px;
  position:absolute;
  right: 180px;
  bottom: -20px;
}
.mirrorImage .timer .timeTitle,
.mirrorImage .timer .totalTime{
  padding: 5px;
  display: flex;
  justify-content: space-between;
}
.mirrorImage .timer .timeTitle .timeHead{
  margin-top: 7px;
  font-family: 'DM Sans';
font-style: normal;
font-weight: 500;
font-size: 12px;
color: #FFFFFF;

}
.mirrorImage .timer .timeTitle .timeHead span{
margin-left: -85px;

}
.mirrorImage .timer .totalTime .timeTable{
  margin-top: -10px;
  font-family: 'DM Sans';
  font-style: normal;
  font-weight: 700;
  font-size: 16px;
  color: #FFFFFF;

}

@media screen and (max-width: 768px) {
  .discoverArt .mirrorImage {
    margin-top: 50px;
    margin-left: 150px;
  }
  .discoverArt .name,
  .discoverArt .description {
    width: 100%;
  }
  .discoverArt .mirrorImage {
    width: 100%;
  }
}
</style>