<template>
  <q-page class="flex flex-center column">
    <div class="row">
    <img
      alt="Quasar logo"
      src="~assets/quasar-logo-vertical.svg"
      style="width: 200px; height: 200px"
    >
    <q-spinner-ball
          color="primary"
          size="2em"
        />
        <q-btn
          :loading="isLoading"
          label="bouwvakker"
          @click="hatsenflats"
        />
      </div>
    <div class="row fit"> 
      <div class="col-12">x</div>
      <div class="col-6">x</div>
      <div class="col-6">x</div>
    </div>

  </q-page>
</template>

<script setup>
import { ref } from 'vue'
     const isLoading = ref(false)
    const hatsenflats = () => {
      isLoading.value = !isLoading.value
    }
</script>