<template>
  <div>
      <v-form>
          <v-text-field
              name="name"
              label="label"
              id="id"
          ></v-text-field>
      </v-form>
  </div>
</template>

<script>
export default {
    data() {
        return {
            name: '',
            label: '',
            id: '',
            }

    }
};
</script>

<style>

</style>
