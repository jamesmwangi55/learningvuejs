<!--change title template-->
<template>
  <div>
    <em>Change the title of your shopping list here</em>
    <input type="text" :value="title" @input="onInput">
  </div>
</template>

<script>
  export default {
    props: ['value', 'title'],
    methods: {
      onInput (event) {
        this.$emit('changeTitle', event.target.value)
      }
    }
  }
</script>

<style scoped>

</style>
