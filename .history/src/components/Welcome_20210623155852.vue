<template id="entry-comp">
  <v-container>
    <v-row class="text-center" style="position:relative; top:300px">
      <v-col cols="12" mb-4>
       <divid="wel">Welcome to <span>Pythos</span></div>
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
#wel {
  color:red
}

</style>