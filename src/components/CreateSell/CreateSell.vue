<template>
  <div class="createSell">
    <div class="container">
      <div class="row">
        <div class="col-12 col-lg-3">
          <div class="firstCol">
            <div class="firstImage">
              <img class="first" :src="img" alt="" />
              <img class="imageIcon" :src="img4" alt="" />
            </div>
            <div class="secondImage">
              <img class="second" :src="img" alt="" />
              <img class="imageIcon" :src="img3" alt="" />
            </div>
          </div>
        </div>
        <div class="col-12 col-lg-3">
          <div class="secondCol">
            <img class="thirdImage" :src="img1" alt="" />
            <img class="imageIcon" :src="img3" alt="" />
          </div>
        </div>
        <div class="col-12 col-lg-6">
          <div class="thirdCol">
            <div>
              <p class="name">Create And Sell Your NFTS</p>
              <p class="description">
                Lorem ipsum dolor sit amet, consectetur adipisicing elit.
                Assumenda, unde, nihil, vitae dolor asperiores inventore
                Assumenda, unde, nihil, vitae dolor asperiores inventore
                delectus rem at repellat
              </p>
              <div class="sellButton">
                <button>Sing Up Now</button>
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
  name: "SingularityTestCreateSell",

  data() {
    return {
      img: "https://i.ibb.co/g9txqbC/image-1-3.png",
      img1: "https://i.ibb.co/GFFbLJ7/image-1-1.png",
      img2: "https://i.ibb.co/4Tw9wJy/image-1-2.png",
      img3:"https://i.ibb.co/gvvGj7g/Ellipse-95.png",
      img4:"https://i.ibb.co/m9dP8mz/Group-105.png",
    };
  },

  mounted() {},

  methods: {},
};
</script>

<style>
.createSell {
  margin-top: 50px;
  margin-bottom: 50px;
}
.createSell .firstCol {
  width: 100%;
}
.createSell .firstCol .firstImage {
  position: relative;
}
.createSell .firstCol .firstImage .imageIcon {
  height: 45px;
  border-radius: 50%;
  position: absolute;
  right: -15px;
  top: 210px;
}
.createSell .firstCol .first {
  width: 100%;
  padding-bottom: 40px;
}
.createSell .firstCol .secondImage{
  width: 100%;
  display: flex;
  justify-content: end;
  position: relative;
}
.createSell .firstCol .secondImage .imageIcon {
  height: 35px;
  border-radius: 50%;
  position: absolute;
  bottom: -13px;
  right: -13px;
}
.createSell .firstCol .secondImage .second {
  height: 170px;
}
.createSell .secondCol,
.createSell .thirdCol {
  height: 100%;
  display: flex;
  place-items: center;
}
.createSell .secondCol{
    position: relative;
}
.createSell .secondCol .imageIcon{
    height: 35px;
    border-radius: 50%;
    position: absolute;
    right: -3px;
    bottom: 105px;
}
.createSell .secondCol img {
  height: 200px;
  margin-left: 20px;
}
.createSell .thirdCol .name {
  width: 200px;
  font-family: "Integral CF";
  font-style: normal;
  font-weight: 700;
  font-size: 23px;
  text-transform: uppercase;
  color: #000000;
}
.createSell .thirdCol .description {
  font-family: "DM Sans";
  font-style: normal;
  font-weight: 400;
  font-size: 18px;
  color: #636363;
}
.createSell .thirdCol p {
  margin: 0;
}
.createSell .thirdCol .sellButton button {
  width: 160px;
  height: 50px;
  margin-top: 10px;
  background: #3d00b7;
  border-radius: 50px;
  border: none;
  font-family: "Averta Demo PE Cutted Demo";
  font-style: normal;
  font-weight: 400;
  font-size: 17px;
  letter-spacing: 0.065em;
  color: #ffffff;
  transition: 0.4s;
}
.createSell .thirdCol .sellButton button:hover {
  background: #8a61dd;
  color: #ffffff;
  font-weight: bold;
}

@media screen and (max-width:768px) {
    .createSell .firstCol .first,
    .createSell .firstCol .second,
    .createSell .secondCol .thirdImage{
        width: 100%;
    }
    .createSell .firstCol .firstImage .imageIcon,
    .createSell .firstCol .secondImage .imageIcon,
    .createSell .secondCol .imageIcon {
        display: none;
      }
      .createSell .secondCol img {
        margin-top: 20px;
        margin-bottom: 20px;
      }
}
</style>