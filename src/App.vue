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
    src: url("./assets/montserrat/montserrat-bold.otf") format("opentype");
  }
  @font-face {
    font-family: Montserrat-semibold;
    src: url("./assets/montserrat/montserrat-semibold.otf") format("opentype");
  }
  @font-face {
    font-family: Montserrat-Medium;
    src: url("./assets/montserrat/montserrat-medium.otf") format("opentype");
  }
  @font-face {
    font-family: Montserrat-Light;
    src: url("./assets/montserrat/montserrat-light.otf") format("opentype");
  }
  @font-face {
    font-family: Montserrat;
    src: url("./assets/montserrat/montserrat-regular.otf") format("opentype");
    font-weight: normal;
  }

  body {
    margin: 0!important;
    font-family: "Montserrat"!important;
    color: black;
  }

  @media only screen and (max-width: 651px) {
    .H1 {
      font-size: 8.4vw!important; 
      line-height: 10.1vw!important;
      margin: 0px!important;
    }

    .H2 {
      font-size: 7.2vw!important;
      line-height: 8.6vw!important;
      margin: 0px!important;
    }

    .H3 {
      font-size: 6vw!important;
      line-hegiht: 7.2vw!important;
      margin: 0px!important;
    }

    .H35 {
      font-size: 5vw!important;
      line-height: 6vw!important;
      margin: 0px!important;
    }

    .H4 {
     font-size: 4.7vw!important;
      line-height: 5.6vw!important;
      margin: 0px!important;
    }

    .H5 {
      font-size: 4.2vw!important;
      line-hegiht: 5vw!important;
      margin: 0px!important;
    }

    .H6 {
      font-size: 4.2vw!important;
      line-hegiht: 5vw!important;
      margin: 0px!important;
    }
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

