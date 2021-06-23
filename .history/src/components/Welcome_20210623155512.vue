<template id="entry-comp">
  <v-container>
    <v-row class="text-center" style="position:relative; top:300px">
      <v-col cols="12" mb-4>
       <div class="hello">Welcome to <span class="hello">Pythos</span></div>
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

<style scoped lang="scss">
#entry-comp {
  font-size: 16px;
}
  .hello {
    font-size: 18px;
  }
</style>