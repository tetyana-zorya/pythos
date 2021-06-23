<template id="entry-comp">
  <v-container>
    <v-row class="text-center position welcome-text">
      <v-col cols="12" mb-4>
       <div>Welcome to <span>Pythos</span></div>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>

  export default {
    name: 'Welcome',

    data: () => ({
      
    }),
  }
</script>

<style>
  .position {
    position:relative; 
    top:300px
  }
  .welcome-text {
    font-size:24px;
  }
</style>