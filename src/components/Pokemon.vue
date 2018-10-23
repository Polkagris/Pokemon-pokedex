<template>
  <div>
    <ul>
    <li v-for="pokemon in pokemans" v-on:click="pokemon.show = !pokemon.show">Name: {{ pokemon.name }}
      <p v-if="pokemon.show">Evolves into: {{ pokemon.next }}</p>
      <div class="card" style="width: 18rem;">
        <img class="card-img-top" v-bind:src="pokemon.imageURL" alt="Card image cap">
        <div class="card-body">
          <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
          <a href="#" class="btn btn-primary">Go somewhere</a>
        </div>
      </div>
    </li>
    </ul>

  </div>
</template>

<script>

export default {
  data () {
    return {
      pokemans: [{name: 'Bulbasaur', next: 'Ivysaur', show: true, imageURL: 'https://vignette.wikia.nocookie.net/pokemon/images/2/21/001Bulbasaur.png/revision/latest/scale-to-width-down/200?cb=20140328190757'},
            {name: 'Ivysaur', next: 'Venosaur', show: false, imageURL: 'https://vignette.wikia.nocookie.net/pokemon/images/7/73/002Ivysaur.png/revision/latest/scale-to-width-down/200?cb=20140328190847'},
            {name: 'Squirtle', next: 'Warturtle', show: false, imageURL: 'https://vignette.wikia.nocookie.net/pokemon/images/3/39/007Squirtle.png/revision/latest/scale-to-width-down/200?cb=20140328191525'},
            {name: 'Charmander', next: 'Charmilion', show: false, imageURL: 'https://vignette.wikia.nocookie.net/pokemon/images/7/73/004Charmander.png/revision/latest/scale-to-width-down/200?cb=20140724195345'},
            {name: 'Charmilion', next: 'Charizard', show: false, imageURL:'https://vignette.wikia.nocookie.net/pokemon/images/4/4a/005Charmeleon.png/revision/latest/scale-to-width-down/200?cb=20140328191309'},
            {name: 'Warturtle', next: 'Blastois', show: false, imageURL:'https://vignette.wikia.nocookie.net/pokemon/images/0/02/009Blastoise.png/revision/latest/scale-to-width-down/200?cb=20140328191642'}]
    }
  },
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
