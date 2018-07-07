<template>
  <v-layout row wrap class="bg__touch">
    <v-flex xs10 offset-xs1 md6 offset-md3 >
      <v-flex xs12 md8 offset-md2 class="maintext__feedback mt-5 mb-5">
        <h1>Stay <span>in touch</span></h1>
      <span class="mt-4 pb-3">This sounded nonsense to Alice, so she said nothing, but set off at once toward the Red Queen. To her surprise, she lost sight of her in a moment.</span>
      </v-flex>
      <v-flex xs12 class="white br__form">
        <v-flex xs10 offset-xs1 class="more__than__mp">
          <form @submit.prevent="validateBeforeSubmit">
            <v-layout xs12 row wrap class="adpt_no_mp">
              <v-flex xs12 md6  class="pr-3">
                <p class="d-flex field__form control has-icon has-icon-right">
                  <input class="palceholder__color" name="email" v-model="email" v-validate="'required|email'" :class="{'input': true, 'is-danger': errors.has('email') }" type="text" placeholder="Email">
                  <i v-show="errors.has('email')" class="fa fa-warning error__red"><span v-show="errors.has('email')" class="help is-danger">{{ errors.first('email') }}</span></i>
                </p>
              </v-flex>
              <v-flex xs12 md6 class="pl-3">
                <p class="d-flex field__form control control has-icon has-icon-right">
                  <input class="palceholder__color" name="name" v-model="name" v-validate="'required|alpha'" :class="{'input': true, 'is-danger': errors.has('name') }" type="text" placeholder="Name">
                  <i v-show="errors.has('name')" class="fa fa-warning error__red"><span v-show="errors.has('name')" class="help is-danger">{{ errors.first('name') }}</span></i>
                </p>
              </v-flex>
              <v-flex xs12 class="message__textarea mt-3">
                <textarea class="palceholder__color" name="text" v-model="message" v-validate="'required'" :class="{'input': true, 'is-danger': errors.has('text') }" type="text" placeholder="Message..."></textarea>
                <i v-show="errors.has('text')" class="fa fa-warning error__red"><span v-show="errors.has('text')" class="help is-danger">{{ errors.first('text') }}</span></i>
              </v-flex>
              <v-flex class="pt-5">
                <button class="download size__style pl-4 pr-4" type="submit">Send Message</button>
              </v-flex>
            </v-layout>
          </form>
        </v-flex>
      </v-flex>
    </v-flex>
  </v-layout>
</template>

<script>
export default {
  name: 'feedback',
  data: () => ({
    email: '',
    name: '',
    message: ''
  }),
  methods: {
    validateBeforeSubmit () {
      this.$validator.validateAll().then((result) => {
        if (result) {
          // eslint-disable-next-line
          alert('Form Submitted!')
          return
        }

        alert('Correct them errors!')
      })
    }
  }
}
</script>

<style>
.bg__touch {
  background-image: url('../assets/img/bg1.png');
  background-repeat: no-repeat;
  background-size: cover;
  height: 100vh;
  align-items: center;
}

.br__form {
  border-radius: 12px;
}

.field__form {
  flex-direction: column;
}

.field__form > input{
  height: 51px;
  border-radius: 6px;
  background-color: #f8f9fa;
  border: solid 1px #e7e8ea;
  font-family: NunitoSans;
  font-size: 17px;
  font-weight: normal;
  font-style: normal;
  font-stretch: normal;
  letter-spacing: normal;
  text-align: left;
  padding-left: 10px;
  color: #000000;
}

.message__textarea > textarea {
  width: 100%;
  border-radius: 6px;
  background-color: #f8f9fa;
  border: solid 1px #e7e8ea;
  height: 211px;
  font-family: NunitoSans;
  font-size: 17px;
  font-weight: normal;
  font-style: normal;
  font-stretch: normal;
  letter-spacing: normal;
  text-align: left;
  color: #000000;
  padding: 10px;
  resize: none;
}

.palceholder__color::-webkit-input-placeholder {
  color: #b9bdc3;
}

.error__red {
  color: red;
  padding-top: 5px;
}

.size__style {
  height: 50px;
  border-radius: 6px;
  font-family: NunitoSans;
  font-size: 17px;
  font-weight: bold;
  font-style: normal;
  font-stretch: normal;
  letter-spacing: 0.9px;
  text-align: center;
  color: #ffffff;
  margin-left: auto;
  margin-right: auto;
  display: block;
}

.more__than__mp {
  padding-top: 80px;
  padding-bottom: 80px;
}

.maintext__feedback > h1 {
  font-family: NunitoSans;
  font-size: 35px;
  font-style: normal;
  font-stretch: normal;
  letter-spacing: 0.9px;
  text-align: center;
  color: #ffffff;
}

.maintext__feedback > h1 > span {
  font-weight: 300;
}

.maintext__feedback > span {
  font-family: NunitoSans;
  font-size: 16px;
  font-weight: normal;
  font-style: normal;
  font-stretch: normal;
  line-height: 1.88;
  letter-spacing: normal;
  text-align: center;
  display: block;
  color: rgba(255, 255, 255, 0.8);
}

@media (max-width: 960px) {
  .adpt_no_mp > div {
    padding-left: 0 !important;
    padding-right: 0 !important;
  }
  .more__than__mp {
    padding: 30px 0;
  }
  .bg__touch {
    height: auto;
    padding-bottom: 40px;
  }
}
</style>
