<template>
  <div>
    <v-container style="position:absolute; top:30px;">
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
