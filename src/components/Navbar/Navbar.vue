<template>
  <div class="fixed-top bg-white">
  <div class="container">
    <nav class="navbar navbar-expand-lg">
      <div class="container-fluid">
        <a class="navBrand" href="#">NFTERS</a>
        <button
          class="navbar-toggler customStyle"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav me-auto mb-2 mb-lg-0">
            <li class="nav-item">
              <a class="nav-link active" aria-current="page" href="#"
                >Marketplace</a
              >
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">Resource</a>
            </li>
            <li class="nav-item">
              <a class="nav-link" href="#">About</a>
            </li>
          </ul>
          <form>
            <div class="d-flex inputField">
              <input
                class="form-control me-2"
                type="search"
                placeholder="Search"
                aria-label="Search"
              />
              <img :src="img" alt="" />
            </div>
          </form>
          <ul class="navbar-nav">
            <li class="nav-item">
              <a class="nav-link linkButton1" href="#">Upload</a>
            </li>
            <li class="nav-item">
              <a class="nav-link linkButton2" href="#">Connect Wallet</a>
            </li>
          </ul>
        </div>
      </div>
    </nav>
</div>
<div>
  <hr>
</div>
</div>
</template>

<script>
export default {
  name: "SingularityTestNavbar",

  data() {
    return {
      img:"https://i.ibb.co/S6BcNjB/search-normal-1-1.png",
    };
  },

  mounted() {},

  methods: {},
};
</script>

<style>
.container{
    margin-top: 10px;
}
.navBrand {
  font-family: "Integral CF";
  font-style: normal;
  font-weight: 700;
  font-size: 24px;
  line-height: 29px;
  text-decoration: none;
  color: #3d00b7;
}
.nav-link {
  margin-left: 30px;
  font-family: "DM Sans";
  font-style: normal;
  font-weight: 500;
  font-size: 16px;
  line-height: 21px;
  letter-spacing: 0.04em;
  color: #000000;
}
.inputField{
  position: relative;
}
.inputField input {
  background: #ffffff;
  border: 2px solid #efefef;
  border-radius: 100px;
}
.inputField img{
  height: 20px;
  position: absolute;
  right: 20px;
  bottom: 10px;
}
.linkButton1 {
  width: 131px;
  margin-top: 10px;
  text-align: center;
  background: #3d00b7;
  border-radius: 60px;
  color: white;
}
.linkButton2 {
  width: 156px;
  margin-top: 10px;
  text-align: center;
  border: 2px solid #3d00b7;
  border-radius: 60px;
  color: #3d00b7;
}

@media screen and (max-width: 768px) {
  .nav-link {
    margin-left: 0px;
  }
  .customStyle{
    background: gray;
    color: white;
  }
}
</style>