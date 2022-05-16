<template>
  <div id="app">
    <HeaderComponent/>
    <main-component/> 
    <footer-component/>
  </div>
</template>

<script>
import HeaderComponent from "./components/HeaderComponent.vue";
import MainComponent from "./components/MainComponent.vue";
import FooterComponent from './components/FooterComponent.vue';

export default {
  name: 'App',
  components: {
    HeaderComponent,
    MainComponent,
    FooterComponent
  }
}
</script>

<style lang="scss">
@import "./style/general.scss";
*{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
.container{
  width: 80%;
  margin: 0 auto ;
}
.debug{
  border:1px solid black;
}

</style>
