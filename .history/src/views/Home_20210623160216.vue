<template>
  <div>
    <v-container>
       <Welcome />
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

</style>
