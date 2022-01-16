<template>
  <div class="BOX-ONE">
    <div class="Header">
      <img class="logo-one" src="../assets/logo.png">
      <div class="nav-buttons">
        <div class="nav-button H5"v-on:click="scrollTo('FAQ')" >FAQ</div>
        <div class="nav-button H5" v-on:click="scrollTo('Curriculum')">Curriculum</div>
        <div class="nav-button H5" v-on:click="scrollTo('Founders')" >Founders</div>
        <div class="Register-button H5" v-on:click="scrollTo('Register-Left')">Register</div>
      </div>
    </div>
    <div class="Content">
      <div class="Content-One">
        <p class="H1 B" style="color: #001B27; padding-bottom: 1%;">Computer Science Mentorship for Calvinist Homeschoolers</p>
        <p class="H35" style="width: 100%;">A proven curriculum to teach your children programming and mathematics taught by a retired software CEO.</p>
        <div class="Content-One-Nav-Button H5" v-on:click="scrollTo('Curriculum')"><div class="buttonC">Our Curriculum</div></div>
      </div>
      <div class="Content-Two">
        <img class="Content-Two-Image" src="../assets/image10.png">
      </div>
    </div>
    <Curriculum></Curriculum>
    <Register></Register>
    <FAQ></FAQ>
    <Founders></Founders>
    <div class="white-space"></div>
  </div>
</template>

<script>
import Curriculum from './Curriculum'
import Register from './Register'
import FAQ from './FAQ'
import Founders from './Founders'

export default {
  name: 'Main',
  components: {
    Curriculum,
    Register,
    FAQ,
    Founders
  },
  data () {
    return {
    }
  },
  methods: {
    scrollTo: (id) => {
      var target = document.getElementById(id)
      var scrollContainer = target;
      do { //find scroll container
          scrollContainer = scrollContainer.parentNode;
          if (!scrollContainer) return;
          scrollContainer.scrollTop += 1;
      } while (scrollContainer.scrollTop == 0);
      
      var targetY = window.screen.height / 0.2;
      do { //find the top of target relatively to the container
          if (target == scrollContainer) break;
          targetY += target.offsetTop;
      } while (target = target.offsetParent);
      
      scroll = function(c, a, b, i) {
          i++; if (i > 30) return;
          c.scrollTop = a + (b - a) / 30 * i;
          setTimeout(function(){ scroll(c, a, b, i); }, 20);
      }
      // start scrolling
      scroll(scrollContainer, scrollContainer.scrollTop, targetY, 0);
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

@media only screen and (max-width: 1007px) {
  .Content-One-Nav-Button {
    width: 80%;
  }
  .nav-buttons {
    width: 50%!important;
  }
}


@media only screen and (max-width: 651px) {
  .Header {
    height: 10%!important;
    position: fixed!important;
    top: 0!important;
  }
  .Content {
    margin-top: 20%!important;
  }
  .Content-Two {
    display: none!important;
  }
  .Register-button {
    width: 27vw!important;
    height: 60%!important;
  }
  .nav-button {
    display: none!important;
  }
  .nav-buttons {
    width: 37vw!important;
  }
  .Content {
    margin-bottom: 50%;
    box-shadow: 0 0 0 0!important;
  }
  .Content-One-Nav-Button {
    width: 95%!important;
    height: 7.5vh!important;
  }
  .buttonC {
    font-size: 5vw!important;
    line-height: 6vw!important;
    margin: 0px!important;
  }

}

.white-space {
  width: 100%;
  height: 5vw;
}

.BOX-ONE {
  width:100vw;
  height:100vh;
}

.Content {
  display: flex;
  flex-direction: row;
  box-shadow: 0 1vw 2vw 0.6vw lightgrey;
}

.Content-One {
  padding-left: 5%;
  margin-top: 5%;
  width: 100%;
  height: 100%;
  padding-bottom: 10%;
}

.Content-One-Nav-Button {
  height: 5vh;
  border-radius: 100px;
  width: 50%;
  text-align: center;
  color: white;
  display: flex;
  margin-top: 5%!important;
  background-color: #00B1FF;
  justify-content: center;
  align-content: center;
  flex-direction: column;
  cursor: pointer;
}

.Content-Two {
  width: 100%;
  height: 100%;
}

.Content-Two-Image {
  width: 70%;
  margin-top: 10%;
  margin-left: 10%;
}

.Header {
  height: 10%;
  width: 100%;
  background-color: #00B1FF;
  display:flex;
}

.logo-one {
  height: 80%;
  margin-left: 5%;
  align-self: center;
}

.nav-buttons {
  font-family: Montserrat-Medium;
  font-size: 1.4vw;
  height: 100%;
  margin-left: auto!important;
  display: flex;
  padding-left: 5%;
  width: 55%;
}

.nav-button {
  align-self: center;
  margin-right: 10%!important;
  text-align: center;
  color: #FFFFFF;
  cursor: pointer;
}

.Register-button {
  align-self: center;
  width: 9vw;
  text-align: center;
  cursor: pointer;
  background-color: white;
  border-radius: 20px;
  display: flex;
  justify-content: center;
  align-content: center;
  flex-direction: column;
  font-size: 1.2vw;
  height: 40%;
  font-family: Montserrat-Medium;
}

</style>
