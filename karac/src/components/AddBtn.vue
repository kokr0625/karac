<template>
  <div class="text-center">
    <v-btn @click="add">
      <v-icon left>mdi-plus</v-icon>Add
    </v-btn>
    <p />
    <component v-for="item in items" :key="item" :is="item"></component>
  </div>
</template>

<script>
import InputForm from "../components/InputForm";
export default {
  data() {
    return {
      items: []
    };
  },
  methods: {
    add() {
      return this.items.push(InputForm);
    }
  },
  components: {
    InputForm
  }
};
</script>

<style>
</style>