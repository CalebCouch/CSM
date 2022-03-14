<template>
  <div class="Curriculum" id="Curriculum">
<!--     <img class="Floating-Image" src="../assets/Illustrations.png">
 -->    <div class="Curriculum-Content">
      <div class="Curriculum-Body">
        <div class="Curriculum-Header">
          <p class="H1 B" style="margin-bottom: 2.5%!important;">Curriculum</p>
          <p class="H4" style="margin-bottom: 4%!important;">The curriculum is designed to teach kids typing, math, VIM, terminal, Javascript, HTML, and CSS. As long as your kids have already learned reading, addition and subtraction they are ready for it.</p>
        </div>
        <div class="Skills-Header">
          <div class="Skills-Header-Text">
            <p class="H2 SB" style="margin-bottom: 2.5%!important;">The Skills</p>
            <p class="H4 M">We start by teaching the kids the six skills required for programming</p>
          </div>
<!--           <img src="../assets/book.png" class="Skills-Header-Image">
 -->        </div>
        <div class="Skills-Body">
          <div class="Skills-Left">
            <p class="H3 Skills-Small-Header">Typing</p>
            <p class="H5 M">When you have solid touch typing skills it makes all computer work, including programming, a lot more fun and interesting.</p>
            <p class="H3 Skills-Small-Header">VIM</p>
            <p class="H5 M">VIM is a set of keyboard shortcuts that make it much faster to write computer programs (or really any text). We use the online game VIM’s Adventures. It's the "Zelda meets text editing" game. So come have some fun and learn some VIM!</p>
            <p class="H3 Skills-Small-Header">Javascript</p>
            <p class="H5 M">Javascript is a popular programming language that is easy to learn and very useful. Almost every website or app you use has at least some javascript code.</p>

          </div>
          <div class="Skills-Right">
            <p class="H3 Skills-Small-Header">Math</p>
            <p class="H5 M">Like everything else in life math is a lot more fun and interesting when you are learning it to solve an interesting problem. Students will learn how and when to use multiplication, division and algebra.</p>
            <p class="H3 Skills-Small-Header">Terminal</p>
            <p class="H5 M">Terminals, also known as command lines or consoles, are used to navigate and manipulate folders and files inside your computer.  When you see a hacker montage in a movie they usually show a screen with a lot of terminal windows open. Not all computer commands are accessible by clicking with a mouse so students will become comfortable with using terminals as they build and release software projects.</p>
            <p class="H3 Skills-Small-Header">HTML & CSS</p>
            <p class="H5 M">HTML and CSS are programming languages used for web-design. We will teach the kids how to use these two languages together to create great user-interfaces.</p>
          </div>
        </div>
        <div class="Projects-Header">
          <p class="H2 SB" style="margin-bottom: 2.5%!important;">The Projects</p>
          <p class="H4 M">After the kids have learned all the essential skills, they will start working on projects designed to further develop their knowledge and ability to program</p>
        </div>
        <div class="Projects-Body" style="margin-bottom: 2.5%!important;">
          <div class="topic">
            <p class="H3 Projects-Small-Header">Complete a Web-Develpment Project</p>
            <p class="H3 Projects-Small-Header">Create a Web-Application</p> 
          </div>
          <div class="topic">
            <p class="H5 Projects-Body-Header">After learning all the basic skills mandatory for programming, the kids will combine their knowledge to create their first project: a functional website.</p>
            <p class="H5 Projects-Body-Header">Your children will now use their web-development, back-end, and database skills to create a web-application</p>
          </div>
          <div class="topic">
            <p class="H3 Projects-Small-Header">Complete a Back-End and Database Project</p>
            <p class="H3 Projects-Small-Header">Contributing to an Open-Source Project</p>
          </div>
          <div class="topic">
            <p class="H5 Projects-Body-Header">In this project, your kids will learn how to set up a database to store data.</p>
            <p class="H5 Projects-Body-Header">Free open-source software is a great way to contribute to something people actually use while learning how to work with others on a large project and begin to establish a reputation as someone that is fun to work with.</p>
          </div>
        </div>
        <div class="Projects-Body2" style="display: none;">
          <p class="H3 Projects-Small-Header">Complete a Web-Develpment Project</p>
          <p class="H5 Projects-Body-Header">After learning all the base skills mandatory for programming, the kids will combine their knowledge to create their first project: a functional website.</p>
          <p class="H3 Projects-Small-Header">Create a Web-Application</p> 
          <p class="H5 Projects-Body-Header">Your children will now use their web-development, back-end, and database skills to create a web-application</p>
          <p class="H3 Projects-Small-Header">Complete a Back-End and Database Project</p>
          <p class="H5 Projects-Body-Header">In this project, your kids will learn how to set up a database to store data in files for any project.</p>
          <p class="H3 Projects-Small-Header">Contributing to an Open-Source Project</p>
          <p class="H5 Projects-Body-Header">Free open-source software is a great way to contribute to something people actually use while learning how to work with others on a large project and begin to establish a reputation.</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Curriculum',
  data () {
    return {
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    @media only screen and (max-width: 651px) {
    .Skills-Body {
      flex-direction: column!important;
    }
    .Skills-Left, .Skills-Right, .Skills-Header-Text {
      width: 100%!important;
    }
    .Projects-Body {
      display: none!important;
    }
    .Projects-Body2 {
      display: flex!important;
    }
    .Projects-Header {
    }
    .Projects-Small-Header {
      width: 100%!important;
    }
    .Projects-Body-Header {
      width: 100%!important;
    }
    .Curriculum-Content {
      box-shadow: 0 -1.2vw 0 0 #D8D8D8!important;
    }
  }


  .Floating-Image {
    top: 120%;
    left: 60%;
    position: absolute;
  }

  .Curriculum {
    width: 100vw;
    display: flex;
    margin-top: 5vw;
  }
  .Curriculum-Content {
    width: 87.5vw;
    margin:auto;
    box-shadow: 0 0 3vw 0.6vw lightgrey;
  }
  .Curriculum-Header {
    width: 100%;
    heigth: 5%;
    margin: auto;
    margin-top: 5%;
    margin-bottom: 5%;
    display: flex;
    text-align: center;
    flex-direction: column;
  }
  .Curriculum-Body {
    width: 85%;
    heigth: 100%;
    margin: auto;
    margin-top: 5%;
    display: flex;
    text-align: center;
    flex-direction: column;
  }
  .Skills-Header {
    text-align: left;
    width: 100%;
    display:flex;
    flex-direction: row;
  }
  .Skills-Header-Text {
    text-align: left;
    width: 60%;
    display:flex;
    flex-direction: column;
  }

  .Skills-Header-Image {
    margin-left: auto;
    width: 25%;
    height: 25%;
  }

  .Skills-Body {
    width: 100%;
    display: flex;
    flex-direction: row;
    margin-top: 2.5%;
  }

  .Projects-Body2 {
    width: 100%;
    display: flex;
    flex-direction: column;
    margin-top: 2.5%;
  }

  .Skills-Left, .Skills-Right {
    width:39%;
    margin-right: auto;
    text-align: left;
  }
  .Skills-Small-Header {
    font-family: 'Montserrat-Medium'!important;
    margin-bottom: 3%!important;
    margin-top: 3%!important;
    color: #00B1FF;
  }

  .Projects-Header {
    text-align: left;
    margin-top: 5%;
    width: 85%;
  }

  .Projects-Text{
    width: 100%;
    display: flex;
    flex-direction: column;
    margin-right: auto;
    text-align: left;
  }

  .Projects-Body{
    width: 100%;
    display: flex;
    flex-direction: column;
    margin-bottom: 15%;
    margin-top: 2.5%;
    text-align: left;
  }
  .Projects-Text-Image {
    display: flex;
    flex-direction: column;
  }

  .Projects-Image {
    margin-top: auto;
    margin-bottom: auto;
  }

  .Projects-Small-Header {
    font-family: 'Montserrat-Medium'!important;
    margin-bottom: 2.5%!important;
    margin-top: 2.5%!important;
    text-align: left;
    color: #00B1FF;
    width: 41%;
    margin-right: auto!important;
  }

  .Projects-Body-Header {
    font-family: 'Montserrat-Medium'!important;
    text-align: left;
    width: 40%;
    margin-right: auto!important;
  }

  .topic {
    display: flex;
    width: 100%;
    flex-direction: row;

  }

</style>
