<template>
  <div class="collectionFeature">
    <div class="container">
      <div class="head">
        <p>Collection Featured NFTS</p>
      </div>
      <div class="row">
        <div v-for="mainImage in mainImages" :key="mainImage.id" class="col-12 col-lg-4">
          <div class="colDesign">
            <div class="firstImage">
              <img :src="mainImage.img" alt="" />
            </div>
            <div>
              <div class="colImages" v-for="image in images" :key="image.id">
                <img :src="image.img" alt="" />
              </div>
            </div>
          </div>
          <p class="title">Amazing Collection</p>
          <div class="colFooter">
            <div class="imageFooter">
              <p><img :src="img3" alt="" /></p>
              <p class="name">by Arkhan</p>
            </div>
            <div>
              <button>Total 54 Items</button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SingularityTestCollectionFetures",

  data() {
    return {
      
      mainImages: [
        { img: "https://i.ibb.co/g9txqbC/image-1-3.png",id:1 },
        { img: "https://i.ibb.co/GFFbLJ7/image-1-1.png",id:2 },
        { img: "https://i.ibb.co/4Tw9wJy/image-1-2.png",id:3 },
      ],
      img3: "https://i.ibb.co/m9dP8mz/Group-105.png",
      images: [
        {
          img: "https://i.ibb.co/VxBR9TG/unsplash-Lpby-DENb-QQg-1.png",
          id: 1,
        },
        {
          img: "https://i.ibb.co/zNTYXh3/unsplash-Lpby-DENb-QQg.png",
          id: 2,
        },
        {
          img: "https://i.ibb.co/c3p814N/unsplash-p-Vo-EPp-Lw818.png",
          id: 3,
        },
      ],
    };
  },

  mounted() {},

  methods: {},
};
</script>

<style>
.collectionFeature {
  background: rgba(217, 224, 236, 0.2);
  padding-bottom: 50px;
}
.collectionFeature .head {
  padding-top: 50px;
  margin-bottom: 30px;
  font-family: "Integral CF";
  font-style: normal;
  font-weight: 700;
  font-size: 28px;
  line-height: 34px;
  color: #000000;
}
.collectionFeature .colDesign {
  display: flex;
}
.collectionFeature .colDesign .firstImage img {
  height: 280px;
  width: 230px;
  margin-right: 10px;
}
.collectionFeature .colDesign .colImages {
  margin-bottom: 10px;
}
.collectionFeature .title {
  margin-top: 15px;
  font-family: "DM Sans";
  font-style: normal;
  font-weight: 700;
  font-size: 20px;
  color: #000000;
}
.collectionFeature .colFooter,
.collectionFeature .colFooter .imageFooter {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.collectionFeature .colFooter .imageFooter img {
  height: 35px;
  border-radius: 50%;
  margin-right: 10px;
}
.collectionFeature .colFooter .imageFooter .name {
  font-family: "DM Sans";
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
  color: #000000;
}
.collectionFeature .colFooter button {
  width: 98px;
  height: 29px;
  margin-right: 20px;
  border: 1px solid #2639ed;
  border-radius: 60px;
  font-family: "DM Sans";
  font-style: normal;
  font-weight: 700;
  font-size: 11.0008px;
  line-height: 14px;
  color: #2639ed;
}

@media screen and(max-width:768px) {
  .collectionFeature .colDesign .firstImage img {
    height: 280px;
    width: 100%;
    margin-right: 10px;
  }
}
</style>