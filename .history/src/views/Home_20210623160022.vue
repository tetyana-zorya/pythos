<template>
  <div>
    <v-container>
       <Welcome />
    </v-container>
    <span class="hi">hi</span>
  </div>
</template>

<script>
  import Welcome from '../components/Welcome'

  export default {
    name: 'Home',

    components: {
      Welcome,
    },
  }
</script>

<style scoped>
.hi {
  color:blue;
}
</style>
