<template>
  <footer class="footer pt-4 my-md-5 pt-md-5">
    <div class="container border-bottom">
      <div class="row">
        <div class="col-12 col-lg-4">
          <h5>NFTERS</h5>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Facilis,
            ipsam in sint aspernatur quod eum odio totam quisquam! Laudantium
          </p>
          <div class="socialIcon">
            <!-- This social icon use as a button -->
            <img :src="img" alt="">
            <img :src="img1" alt="">
            <img :src="img2" alt="">
          </div>
        </div>
        <div class="col-12 col-lg-2">
          <h5>Market Place</h5>
          <ul class="list-unstyled text-small">
            <li class="mb-1">
              <a class="link-secondary text-decoration-none" href="#"
                >All NFTs</a
              >
            </li>
            <li class="mb-1">
              <a class="link-secondary text-decoration-none" href="#">New</a>
            </li>
            <li class="mb-1">
              <a class="link-secondary text-decoration-none" href="#">Art</a>
            </li>
            <li class="mb-1">
              <a class="link-secondary text-decoration-none" href="#">Sports</a>
            </li>
            <li class="mb-1">
              <a class="link-secondary text-decoration-none" href="#"
                >Utility</a
              >
            </li>
            <li class="mb-1">
              <a class="link-secondary text-decoration-none" href="#">Music</a>
            </li>
            <li class="mb-1">
              <a class="link-secondary text-decoration-none" href="#"
                >Domain Name</a
              >
            </li>
          </ul>
        </div>
        <div class="col-12 col-lg-2">
          <h5>My Account</h5>
          <ul class="list-unstyled text-small">
            <li class="mb-1">
              <a class="link-secondary text-decoration-none" href="#"
                >Profile</a
              >
            </li>
            <li class="mb-1">
              <a class="link-secondary text-decoration-none" href="#"
                >Favorite</a
              >
            </li>
            <li class="mb-1">
              <a class="link-secondary text-decoration-none" href="#"
                >My Collection</a
              >
            </li>
            <li class="mb-1">
              <a class="link-secondary text-decoration-none" href="#"
                >Settings</a
              >
            </li>
          </ul>
        </div>
        <div class="col-12 col-lg-4">
          <h5>Stay In The Loop</h5>
          <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Dicta
            doloribus id consequatur eligendi, dolorum laboriosam deserunt,
            ratione
          </p>
          <div class="submitForm">
            <input type="text" placeholder="Enter your email address.." />
            <button>Subscribe Now</button>
          </div>
        </div>
      </div>
    </div>
    <div class="copyRight">
      <p>Copyright @ 2022 Avi Yansah</p>
    </div>
  </footer>
</template>

<script>
export default {
  name: "SingularityTestFooter",

  data() {
    return {
      img: "https://i.ibb.co/HnX93z2/Group-1.png",
      img1: "https://i.ibb.co/8dy07qB/Group-2.png",
      img2: "https://i.ibb.co/5TRd97y/Group.png",
    };
  },

  mounted() {},

  methods: {},
};
</script>

<style>
.footer .socialIcon img{
margin-right: 20px;
cursor: pointer;
}
.footer .socialIcon img:hover{
transform: scale(.9);
}
.footer .submitForm {
  position: relative;
}
.footer .submitForm input {
  width: 350px;
  height: 60.79px;
  padding-left: 20px;
  background: #ffffff;
  border: 2px solid #f1f1f1;
  border-radius: 45.595px;
}
.footer .submitForm button {
  width: 120.79px;
  height: 46.4px;
  background: #2639ed;
  border: none;
  border-radius: 45.595px;
  color: white;
  position: absolute;
  right: 10px;
  bottom: 8px;
  transition: 0.4s;
}
.footer .submitForm button:hover {
  background: none;
  border:1px solid #2639ed;
  color: black;
}
.footer .copyRight {
  margin-top: 20px;
  text-align: center;
  font-family: "Averta Demo PE Cutted Demo";
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  color: #a4a4a4;
}
</style>