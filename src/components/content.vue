<template>
  <div class="content">
    <v-sheet class="w-100">
      <v-form @submit.prevent>
        <v-text-field
          v-model="form.firstName"
          :rules="form.rules"
          label="First name"
          class="mt-4 w-100"
        ></v-text-field>

        <v-text-field
          v-model="form.firstName"
          :rules="form.rules"
          label="First name"
          class="mt-4 w-100"
        ></v-text-field>

        <v-text-field
          v-model="form.firstName"
          :rules="form.rules"
          label="First name"
          class="mt-4 w-100"
        ></v-text-field>

        <v-text-field
          v-model="form.firstName"
          :rules="form.rules"
          label="First name"
          class="mt-4 w-100"
        ></v-text-field>
        <v-btn class="mt-2" type="submit" block>Submit</v-btn>
      </v-form>
    </v-sheet>
  </div>
</template>
<script lang="ts" setup>
import { reactive } from "vue";

const form = reactive({
  firstName: "",
  rules: [
    (value) => {
      if (value) return true;

      return "You must enter a first name.";
    },
  ],
});
</script>
<style lang="scss" scoped>
@import "../assets//main.scss";
</style>
