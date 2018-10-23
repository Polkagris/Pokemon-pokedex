<template>
  <header>
    <h1>{{ title }}
        <img id="icon" v-bind:src="this.iconURL"></img>
    </h1>
  </header>
</template>

<script>

export default {
  props: ["title", "iconURL"],
  data () {
    return {

    }
  }
}
</script>

<style>
h1{
  padding: 20px;
  background-color: #00c10f;
  text-align: center;
  color: white;
}
#icon{
  height: 50px;
}
</style>
