<template>
  <div>
    <app-header v-bind:title="title" v-bind:iconURL="iconURL"></app-header>
    <app-body v-bind:pokemans="pokemans"></app-body>
    <app-footer v-bind:msg="msg"></app-footer>
  </div>
</template>

<script>
import msg from './components/Footer.vue';
import title from './components/Header.vue';
import pokemans from './components/Pokemon.vue'

export default {
  components: {
    'app-footer': msg,
    'app-header': title,
    'app-body': pokemans
  },
  data () {
    return {
      pokemans: [{name: 'Bulbasaur', type: 'grass', next: 'Ivysaur', show: true, imageURL: 'https://vignette.wikia.nocookie.net/pokemon/images/2/21/001Bulbasaur.png/revision/latest/scale-to-width-down/200?cb=20140328190757'},
            {name: 'Ivysaur', type: 'grass', next: 'Venosaur', show: false, imageURL: 'https://vignette.wikia.nocookie.net/pokemon/images/7/73/002Ivysaur.png/revision/latest/scale-to-width-down/200?cb=20140328190847'},
            {name: 'Warturtle', type: 'water', next: 'Blastois', show: false, imageURL:'https://vignette.wikia.nocookie.net/pokemon/images/0/0c/008Wartortle.png/revision/latest/scale-to-width-down/200?cb=20140328191553'},
            {name: 'Squirtle', type: 'water', next: 'Warturtle', show: false, imageURL: 'https://vignette.wikia.nocookie.net/pokemon/images/3/39/007Squirtle.png/revision/latest/scale-to-width-down/200?cb=20140328191525'},
            {name: 'Charmander', type: 'fire', next: 'Charmilion', show: false, imageURL: 'https://vignette.wikia.nocookie.net/pokemon/images/7/73/004Charmander.png/revision/latest/scale-to-width-down/200?cb=20140724195345'},
            {name: 'Charmilion', type: 'fire', next: 'Charizard', show: false, imageURL:'https://vignette.wikia.nocookie.net/pokemon/images/4/4a/005Charmeleon.png/revision/latest/scale-to-width-down/200?cb=20140328191309'},
            {name: 'Blastois', type: 'water', next: 'none', show: false, imageURL:'https://vignette.wikia.nocookie.net/pokemon/images/0/02/009Blastoise.png/revision/latest/scale-to-width-down/200?cb=20140328191642'}],

      msg: 'Made with <3 by Arne',
      title: 'Pokemon',
      iconURL: 'https://cdn.pixabay.com/photo/2016/07/23/13/18/pokemon-1536849_960_720.png'
    }
  }
}
</script>

<style>

</style>
