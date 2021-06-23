<template>
  <div>
    <v-container>
       <Welcome />
       <span class="hi">hi</span>
    </v-container>
    
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
