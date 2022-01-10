<template>
  <div class="Founders" id="Founders">
    <div class="Founders-Content">
      <div class="Founders-Body">
        <div class="Founders-Header">
          <p class="H1 B" style="color: #00B1FF;">Founders</p>
          <div class="Founders-People">
            <div class="Person">
              <img src="../assets/JackCouch.png">
              <p class="H5" style="color: #6A6A6A;">Jack is a succesful software and computer science engineer. He founded this program to provide kids with benifital skills that can be put towards a lucrative career</p>
              
            </div>
            <div class="Person">
              <img src="../assets/CalebCouch.png">
              <p class="H5" style="color: #6A6A6A;">Jack is a succesful software and computer science engineer. He founded this program to provide kids with benifital skills that can be put towards a lucrative career</p>
              
            </div>
            <div class="Person">
              <img src="../assets/EllaCouch.png">
              <p class="H5" style="color: #6A6A6A;">Designed the website, And wanted to be included in the founders section.</p>
              
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Founders',
  data () {
    return {
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .Founders {
    width: 100vw;
    height: 40vw;
    display: flex;
    margin-top: 5vw;
  }
  .Founders-Content {
    width: 87.5vw;
    margin:auto;
    box-shadow: 0 0 3vw 0.6vw lightgrey;
  }

  @media only screen and (max-width: 651px) {
    .Founders-People {
      flex-direction: column!important;
    }
    .Person {
      width: 100%!important;
    }
  }

  .Founders-Header {
    width: 100%;
    heigth: 5%;
    margin: auto;
    margin-top: 5%;
    margin-bottom: 5%;
    display: flex;
    text-align: center;
    flex-direction: column;
  }
  .Founders-Body {
    width: 77.5%;
    heigth: 100%;
    margin: auto;
    margin-top: 5%;
    display: flex;
    text-align: center;
    flex-direction: column;
  }
  .Founders-People {
    display: flex;
    flex-direction: row;
    margin-top: 5%;
  }
  .Person {
    margin-top: 0!important;
    width: 30%;
    display: flex;
    flex-direction: column;
    margin: auto;
  }
</style>
