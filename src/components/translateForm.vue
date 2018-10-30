<template>
  <div id="translateForm">
      <form v-on:submit="formSubmit">
          <input type="text" v-model="textToTranslate" placeholder="please input">
          <select name="" id="">
              <option value="en">english</option>
          </select>
          <input type="submit" value="翻译">
      </form>
  </div>
</template>

<script>
export default {
  name: 'translateForm',
  data: function () {
    return {
      textToTranslate: ''
    }
  },
  methods: {
    formSubmit: function (e) {
      this.$emit('formSubmit', this.textToTranslate)
      e.preventDefault()
    }
  }
}
</script>
