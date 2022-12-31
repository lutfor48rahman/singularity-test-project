<template>
  <div class="discoverGallery">
    <div class="row">
      <div v-for="image in images" :key="image.id" class="col-12 col-lg-3">
        <div class="imageBox">
          <div class="images">
            <img class="mainImage" :src="image.img" alt="" />
            <div class="bubbleImage">
              <img :src="img2" alt="" />
              <img :src="img1" alt="" />
              <img :src="img2" alt="" />
              <img :src="img1" alt="" />
            </div>
          </div>
          <div class="mid">
            <p class="name">ArtCrypto</p>
          </div>

          <div class="count">
            <p><img :src="icon" alt="" /> 0.25 ETH</p>
            <p>1 of 321</p>
          </div>
          <div class="countTime">
            <p>3h 50m 2s left</p>
            <p>Place a bid</p>
          </div>
        </div>
      </div>
    </div>
    <div class="galleyButton">
      <button>More NFTs</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "SingularityTestDiscoverGallery",

  data() {
    return {
      // img: "https://i.ibb.co/g9txqbC/image-1-3.png",
      // img1: "https://i.ibb.co/GFFbLJ7/image-1-1.png",
      // img2: "https://i.ibb.co/4Tw9wJy/image-1-2.png",
      img: "https://i.ibb.co/xzsmchL/Ellipse-95-1.png",
      img1: "https://i.ibb.co/QkFLryp/Ellipse-95-2.png",
      img2: "https://i.ibb.co/9GtZVMh/Ellipse-95-3.png",
      icon: "https://i.ibb.co/h819ydL/ethereum-1.png",
      images: [
        { img: "https://i.ibb.co/g9txqbC/image-1-3.png", id: 1 },
        { img: "https://i.ibb.co/GFFbLJ7/image-1-1.png", id: 2 },
        { img: "https://i.ibb.co/4Tw9wJy/image-1-2.png", id: 3 },
        { img: "https://i.ibb.co/g9txqbC/image-1-3.png", id: 1 },
        { img: "https://i.ibb.co/GFFbLJ7/image-1-1.png", id: 2 },
        { img: "https://i.ibb.co/4Tw9wJy/image-1-2.png", id: 3 },
        { img: "https://i.ibb.co/g9txqbC/image-1-3.png", id: 1 },
        { img: "https://i.ibb.co/GFFbLJ7/image-1-1.png", id: 2 },
        { img: "https://i.ibb.co/4Tw9wJy/image-1-2.png", id: 3 },
        { img: "https://i.ibb.co/g9txqbC/image-1-3.png", id: 1 },
        { img: "https://i.ibb.co/GFFbLJ7/image-1-1.png", id: 2 },
        { img: "https://i.ibb.co/4Tw9wJy/image-1-2.png", id: 3 },
      ],
    };
  },

  mounted() {},

  methods: {},
};
</script>

<style>
.discoverGallery {
  margin-top: 40px;
}
.discoverGallery .imageBox {
  padding: 5px;
  margin-bottom: 20px;
  background: #ffffff;
  border: 1.09706px solid rgba(242, 242, 242, 0.5);
  border-radius: 13.1647px;
}
.discoverGallery .imageBox .images .mainImage {
  width: 100%;
}
.discoverGallery .imageBox .images {
  width: 100%;
  position: relative;
}
.discoverGallery .imageBox .images .bubbleImage {
  position: absolute;
  left: 10px;
  bottom: -10px;
}
.discoverGallery .bubbleImage img {
  height: 35px;
  border-radius: 50%;
}
.discoverGallery .bubbleImage img:nth-child(2),
.discoverGallery .bubbleImage img:nth-child(3),
.discoverGallery .bubbleImage img:nth-child(4) {
  margin-left: -15px;
}
.discoverGallery .mid .name {
  margin: 0;
  margin-top: 15px;
  margin-bottom: 5px;
  font-family: "DM Sans";
  font-style: normal;
  font-weight: 700;
  font-size: 19.7471px;
  color: #000000;
}
.discoverGallery .count,
.discoverGallery .countTime {
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.discoverGallery .count p:nth-child(1) {
  font-family: "DM Sans";
  font-style: normal;
  font-weight: 700;
  font-size: 10.9706px;
  color: #00ac4f;
}
.discoverGallery .count p:nth-child(2) {
  font-family: "DM Sans";
  font-style: normal;
  font-weight: 700;
  font-size: 10.9706px;
}
.discoverGallery .count img {
  height: 15px;
  margin-top: -5px;
}
.discoverGallery .countTime p {
  font-family: "DM Sans";
  font-style: normal;
  font-weight: 500;
  font-size: 12.3588px;
  color: #4f33a3;
}
.discoverGallery .countTime p:nth-child(1) {
  padding: 5px;
  background: #f5f5f5;
  border-radius: 109.706px;
}
.discoverGallery .galleyButton{
  margin-top: 30px;
  padding-bottom: 40px;
  text-align: center;
}
.discoverGallery .galleyButton button{
  width: 179px;
height: 56px;
text-align: center;
border: 2px solid #3D00B7;
border-radius: 50px;
transition: 0.4s;
}
.discoverGallery .galleyButton button:hover{
background:#3D00B7;
color: white;

}
</style>