<template>
  <div class="hello">
    <h2>{{ msg }}</h2>
    <h4>{{ email }}</h4>
    <p><span v-html="rawHtml"></span></p>
  </div>
</template>

<script>
export default {
    name: "HelloWorld",
    props: {
        msg: String,
        email: String,
        rawHtml: HTMLElement
    },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
