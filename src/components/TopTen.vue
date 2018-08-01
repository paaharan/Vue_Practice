<template>
  <v-layout row wrap align-center>
    <v-flex v-for="(item, index) in topten">
      <v-card width="200px" height="300px" style="line-height: 30px; text-align: center; font-size: 20px"  >
        <a v-bind:href="item.link" style="text-decoration: none; color: black;"> <v-card-text>{{index + 1}} {{item.title}}</v-card-text></a>
      </v-card>
    </v-flex>
  </v-layout>
</template>

<script>
    export default {
        name: "TopTen",
      props: ["topten"]
    }
</script>

<style scoped>

</style>
