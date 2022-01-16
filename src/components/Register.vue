<template>
  <div class="Register" id="Register">
    <div class="Register-Content">
      <div class="Register-Left">
        <p class="H1 B" style="margin-top: 12.5%!important; margin-bottom: 2.5%!important;">Register</p>
        <p class="H6 L" style="width: 80%;">Each student is required to be between the ages of eight and eighteen, have the skill to read, have the skill to do addition and subtraction math problems, and be part of a Reformed, Christian, family. </p>
        <div class="Form">
          <b-form @submit="onSubmit" @reset="onReset" v-if="show">
            <p class="H6 M form-header">Parent’s Full Name</p>
            <b-form-input
              id="input-1"
              v-model="form.name"
              type="text"
              name="name"
              required
            ></b-form-input>

            <p class="H6 M form-header">Parent’s Phone Number</p>
            <b-form-input
              id="input-1"
              v-model="form.number"
              type="text"
              name="number"
              required
            ></b-form-input>

             <p class="H6 M form-header">Parent’s Email</p>
            <b-form-input
              id="input-1"
              v-model="form.email"
              type="email"
              name="email"
              required
            ></b-form-input>

             <p class="H6 M form-header" style="width: 80%;">Please Enter the Ages of all Kids 
You are Wanting to Participater</p>
            <b-form-input
              id="input-1"
              v-model="form.ages"
              type="text"
              name="ages"
              required
            ></b-form-input>
            <b-button type="submit" class="Register-Button">Register Now</b-button>
          </b-form>
         <!--  <b-card class="mt-3" header="Form Data Result">
            <pre class="m-0">{{ form }}</pre>
          </b-card> -->
        </div>
        
      </div>
      <div class="Register-Right">
        <img src="../assets/computer2.png" class="computer2"></div>
        
      </div>
    </div>
  </div>
</template>

<script>
import emailjs from '@emailjs/browser';
export default {
  name: 'Register',
  data () {
    return {
      form: {
          email: '',
          name: '',
          number: '',
          ages: ''
        },
        show: true
    }
  },
  methods: {
    onSubmit(e) {
      e.preventDefault()
      try {
        emailjs.sendForm('service_octa5y8', 'template_xt0910h', e.target,
        'user_zU5VyI9YLll168gj1DPex', {
          name: this.name,
          email: this.email,
          number: this.number,
          ages: this.ages
        })
        alert('registration successful')
      } catch(error) {
          console.log({error})
      }
      // Reset form field
      this.name = ''
      this.email = ''
      this.name = ''
      this.ages = ''

    },
    onReset(event) {
      event.preventDefault()
      // Reset our form values
      this.form.name = ''
      this.form.number = 0
      this.form.email = ''
      this.form.ages = ''
      // Trick to reset/clear native browser form validation state
      this.show = false
      this.$nextTick(() => {
        this.show = true
      })
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

  @media only screen and (max-width: 651px) {
    .Register-Left {
      box-shadow: 0 -1.2vw 0 0 #D8D8D8!important;
    }
  }
  @media only screen and (max-width: 800px) {
    .Register-Right {
      display: none;
    }
    .Register-Left {
      width: 100%!important;
    }
  }
  .computer2 {
    width: 100%;
    height: 100%;
  }

  .Register-Button {
    border: 0px;
    height: 5vh;
    border-radius: 100px;
    width: 100%;
    align-items: center;
    text-align: center;
    color: white;
    display: flex;
    margin-top: 5%;
    margin-bottom: 5%;
    background-color: #00B1FF;
    justify-content: center;
    align-content: center;
    flex-direction: column;
    cursor: pointer;
  }

  .form-header {
    text-align: left;
    margin-top: 5% !important;
    margin-bottom: 2.5%!important;
  }

  .Register {
    width: 100vw;
    display: flex;
    margin-top: 5vw;
  }

  .Register-Content {
    width: 87.5vw;
    margin:auto;
    display: flex;
    flex-direction: row;
  }

  .Register-Left, Register-Right {
  }

  .Register-Right {
    width: 55%;
  }

  .Register-Left {
    width: 45%;
    display: flex;
    flex-direction: column;
    text-align: center;
    align-items: center;
    box-shadow: 0 0 3vw 0.6vw lightgrey;
  }

  .Form {
    width: 60%;
    margin: auto;
    margin-top: 5%;
    margin-bottom: 10%;
  }

</style>
