<template>
  <v-container class="mt-10">
    <v-row>
      <v-col cols="12" sm="6">
        <v-slider
          v-model="value"
          color="blue"
          thumb-label
          label="Slider"
        ></v-slider>
      </v-col>

      <v-col cols="12" sm="6">
        <v-text-field
          v-model="value"
          label="Caja de texto"
          type="number"
        ></v-text-field>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import { ref } from 'vue'

export default {
  setup() {
    const value = ref(50)

    return {
      value
    }
  }
}
</script>

