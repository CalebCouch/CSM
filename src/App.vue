<template>
  <div id="app">
    <Main/>
  </div>
</template>

<script>
import Main from './components/Main'

export default {
  name: 'App',
  components: {
    Main
  }
}
</script>

<style>
  @font-face {
    font-family: Montserrat;
    font-weight: bold;
    src: url("./assets/Montserrat/Montserrat-Bold.otf") format("opentype");
  }
  @font-face {
    font-family: Montserrat-semibold;
    src: url("./assets/Montserrat/Montserrat-Semibold.otf") format("opentype");
  }
  @font-face {
    font-family: Montserrat-Medium;
    src: url("./assets/Montserrat/Montserrat-Medium.otf") format("opentype");
  }
  @font-face {
    font-family: Montserrat-Light;
    src: url("./assets/Montserrat/Montserrat-Light.otf") format("opentype");
  }
  @font-face {
    font-family: Montserrat;
    src: url("./assets/Montserrat/Montserrat-Regular.otf") format("opentype");
    font-weight: normal;
  }

  body {
    margin: 0!important;
    font-family: "Montserrat"!important;
    color: black;
  }

  .H1 {
    font-size: 4.2vw; 
    line-height: 5.1vw;
    margin: 0px!important;
  }

  .H2 {
    font-size: 3.6vw;
    line-height: 4.3vw;
    margin: 0px!important;
  }

  .H3 {
    font-size: 2.7vw;
    line-hegiht: 3.29vw;
    margin: 0px!important;
  }

  .H35 {
    font-size: 2.4vw;
    line-height: 2.925vw;
    margin: 0px!important;
  }

  .H4 {
    font-size: 1.8vw;
    line-hegiht: 2.1vw;
    margin: 0px!important;
  }

  .H5 {
    font-size: 1.4vw;
    line-hegiht: 1.7vw;
    margin: 0px!important;
  }

  .H6 {
    font-size: 1.15vw;
    line-hegiht: 1.3vw;
    margin: 0px!important;
  }

  .B {
    font-family: 'Montserrat';
    font-weight: bold;
  }

  .SB {
    font-family: 'Montserrat-semibold'!important;
  }

  .M {
    font-family: 'Montserrat-Medium'!important;
  }

  .L {
    font-family: 'Montserrat-Light'!important;
  }

</style>

