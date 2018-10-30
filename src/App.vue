<template>
  <div id="app">
    <h1>****</h1>
    <h5>easy/easy/easy</h5>
    <translateForm v-on:formSubmit="translateText"></translateForm>
    <translateOutput v-text="translatedText"></translateOutput>
    <button-xc msg="注册" :isShow="true"></button-xc>
    <button-xc msg="登录" :isShow="true"></button-xc>
    <buttonDIY></buttonDIY>
  </div>
</template>

<script>
import TranslateForm from './components/translateForm'
import TranslateOutput from './components/translateOutput'
import buttonDIY from './components/button'

export default {
  name: 'app',
  data: function () {
    return {
      translatedText: ''
    }
  },
  components: {
    TranslateForm,
    TranslateOutput,
    buttonDIY
  },
  methods: {
    translateText: function (text) {
      // alert(text)
      this.translatedText = 'xc'
    }
  }
}
</script>
