<template>
  <v-app id="app">
    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script>



export default {
  name: 'App',

  data: () => ({
    //
  }),
};
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Stoke:wght@300&display=swap');

#app {
font-size:16px;
}
</style>
