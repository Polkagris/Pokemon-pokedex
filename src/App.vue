<template>
  <div>
    <app-header></app-header>
    <app-body></app-body>
    <app-footer></app-footer>
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

    }
  }
}
</script>

<style>

</style>
