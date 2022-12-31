<template>
  <Navbar/>
  <ArtDiscoverVue/>
  <AboutNFTVue/>
  <TopCollection/>
  <CollectionFeturesVue/>
  <CreateSellVue/>
  <MoreDiscoverVue/>
  <FooterVue/>
</template>

<script>
import Navbar from './components/Navbar/Navbar.vue'
import ArtDiscoverVue from './components/ArtDiscover.vue';
import AboutNFTVue from './components/AboutNFT.vue';
import TopCollection from './components/TopCollection/TopCollection.vue';
import CollectionFeturesVue from './components/CollectionFetures/CollectionFetures.vue';
import CreateSellVue from './components/CreateSell/CreateSell.vue';
import MoreDiscoverVue from './components/MoreDiscover/MoreDiscover.vue';
import FooterVue from './components/Footer/Footer.vue';
export default {
  name: 'App',
  components: {
    Navbar,
    ArtDiscoverVue,
    AboutNFTVue,
    TopCollection,
    CollectionFeturesVue,
    CreateSellVue,
    MoreDiscoverVue,
    FooterVue
  }
}
</script>

<style>
 *{
  margin: 0;
  padding:0;
 }
 body{
  overflow-x: hidden;
 }
</style>
