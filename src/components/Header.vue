<template>
  <header>
    <h1>{{ title }}
        <img id="icon" v-bind:src="this.iconURL"></img>
    </h1>
  </header>
</template>

<script>

export default {
  data () {
    return {
      title: 'Pokemon',
      iconURL: 'https://cdn.pixabay.com/photo/2016/07/23/13/18/pokemon-1536849_960_720.png'
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
