<template>
  <v-col cols="4">
    <v-card class="mx-auto" raised>
      <v-img :src="src" height="200px" class="white--text">
        <v-card-title class="align-end fill-height">Title</v-card-title>
      </v-img>
      <v-card-text>
        <div>description</div>
      </v-card-text>
      <v-card-actions>
        <v-btn flat color="primary">text</v-btn>
        <v-btn flat color="primary">text</v-btn>
      </v-card-actions>
    </v-card>
  </v-col>
</template>

<script>
export default {
  data() {
    return {
      src:
        "https://cdn.pixabay.com/photo/2019/09/13/20/26/bridges-4474817__340.jpg"
    };
  }
};
</script>

<style>
</style>