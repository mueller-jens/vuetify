<template>
  <v-container fluid>
    <v-radio-group v-model="column">
      <v-radio
        label="Option 1"
        value="radio-1"
      ></v-radio>
      <v-radio
        label="Option 2"
        value="radio-2"
      ></v-radio>
    </v-radio-group>
    <hr>
    <v-radio-group
      v-model="inline"
      inline
    >
      <v-radio
        label="Option 1"
        value="radio-1"
      ></v-radio>
      <v-radio
        label="Option 2"
        value="radio-2"
      ></v-radio>
    </v-radio-group>
  </v-container>
</template>

<script setup>
  import { ref } from 'vue'

  const column = ref(null)
  const inline = ref(null)
</script>

<script>
  export default {
    data () {
      return {
        column: null,
        inline: null,
      }
    },
  }
</script>
