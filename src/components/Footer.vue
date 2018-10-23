<template>
  <footer>
    <p>{{ msg }}</p>
  </footer>
</template>

<script>
export default {
  props: ["msg"],
  data () {
    return {

    }
  }
}
</script>

<style scoped>
p{
  color: white;
  background-color: #ef832b;
  padding: 10px;
  text-align: center;
}
</style>
