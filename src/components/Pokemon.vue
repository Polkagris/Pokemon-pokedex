<template>
  <div>
    <ul>
    <li v-for="pokemon in pokemans" v-on:click="pokemon.show = !pokemon.show">Name: {{ pokemon.name }}
      <div class="card" style="width: 18rem;">
        <img class="card-img-top" v-bind:src="pokemon.imageURL" alt="Card image cap">
        <div class="card-body">
          <p class="card-text">{{ pokemon.type}}</p>
          <a href="#" class="btn btn-primary">Go somewhere</a>
          <p v-if="pokemon.show">Evolves into: {{ pokemon.next }}</p>
        </div>
      </div>
    </li>
    </ul>
  </div>
</template>

<script>

export default {
  props: ['pokemans'],

  data () {
    return {

    }
  }
}
</script>

<style scoped>
ul{
  display: flex;
  flex-wrap: wrap;
}

li{
  flex-grow: 1;
  padding: 30px;
  border: 1px solid black;
  list-style-type: none;
  text-align: center;
}
</style>
