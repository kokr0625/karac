<template>
  <v-container grid-list-xs>
    <v-btn class="text-center" @click="add">
      <v-icon left>mdi-plus</v-icon>Add
    </v-btn>
    <p />
    <v-row>
      <v-col cols="4">
        <input-form v-for="item in items" :key="item" :is="item"></input-form>
      </v-col>
    </v-row>
    <card-frame></card-frame>
  </v-container>
</template>

<script>
import InputForm from "./InputForm";
import CardFrame from "./CardFrame";

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
    InputForm,
    CardFrame
  }
};
</script>

<style>
</style>
