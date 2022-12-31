<template>
  <div class="discoverMore">
    <div class="container">
      <div class="title">
        <p>Discover More NFTS</p>
      </div>
      <div class="subNav">
        <ul>
          <li class="activeLi">
            <a href="#">All Categories</a>
          </li>
          <li>
            <a href="#"> Art</a>
          </li>
          <li>
            <a href="#">Celebrities</a>
          </li>
          <li>
            <a href="#">Gaming</a>
          </li>
          <li>
            <a href="#">Sport</a>
          </li>
          <li>
            <a href="#">Music</a>
          </li>
          <li>
            <a href="#">Crypto</a>
          </li>
        </ul>
        <div class="filterIcon">
          <button class="filterButton">
            <img :src="icon" alt="" />
            <p>All Filter</p>
          </button>
        </div>
      </div>
      <discoverGallery />
    </div>
  </div>
</template>

<script>
import discoverGallery from "../MoreDiscover/DiscoverGallery.vue";
export default {
  name: "SingularityTestMoreDiscover",
  components: {
    discoverGallery,
  },
  data() {
    return {
      icon: "https://i.ibb.co/LnmQ7BB/filter-results-button-1.png",
    };
  },

  mounted() {},

  methods: {},
};
</script>

<style>
.discoverMore {
  margin-top: 30px;
  margin-bottom: 30px;
  background: rgba(217, 224, 236, 0.2);
}
.discoverMore .title p {
  padding-top: 40px;
  font-family: "Integral CF";
  font-style: normal;
  font-weight: 700;
  font-size: 30px;
  color: #000000;
}
.discoverMore .subNav,
.discoverMore .subNav ul {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.discoverMore .subNav ul {
  margin: 0;
  padding: 0;
  list-style: none;
}
.discoverMore .subNav ul li {
  margin-right: 40px;
  height: 45px;
  background: rgba(220, 220, 220, 0.2);
  border-radius: 100px;
  display: flex;
  align-items: center;
  transition: 0.4s;
}
.discoverMore .subNav ul li:hover {
  background: #483966;
  font-weight: 500;
}
.discoverMore .subNav ul .activeLi {
  margin-right: 40px;
  height: 45px;
  background: #3d00b7;
  border-radius: 100px;
  display: flex;
  align-items: center;
}
.discoverMore .subNav ul .activeLi a {
  font-family: "DM Sans";
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
  color: white;
}
.discoverMore .subNav ul li a {
  text-decoration: none;
  padding: 10px;
  font-family: "DM Sans";
  font-style: normal;
  font-weight: 500;
  font-size: 14px;
  color: #000000;
}
.discoverMore .subNav .filterIcon {
  display: flex;
  align-items: center;
  transition: 0.4s;
}
.discoverMore .subNav .filterIcon:hover {
  background: #483966;
  border-radius: 100px;
}
.discoverMore .subNav .filterIcon img {
  height: 20px;
  margin-right: 5px;
}

.discoverMore .subNav .filterIcon .filterButton p {
  margin: 0;
  padding: 0;
}
.discoverMore .subNav .filterIcon .filterButton {
  background: rgba(220, 220, 220, 0.2);
  border-radius: 100px;
  border: none;
  padding: 10px;
  display: flex;
  align-items: center;
}

@media screen and (max-width:768px) {
  .discoverMore .subNav ul{
    display: grid;
    grid-auto-columns: row;
  }
}
</style>