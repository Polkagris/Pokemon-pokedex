<template>
  <footer>
    <p>{{ msg }}</p>
  </footer>
</template>

<script>
export default {
  data () {
    return {
      msg: 'Made with <3 by Arne'
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
