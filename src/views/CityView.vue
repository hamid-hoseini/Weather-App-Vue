<template>
  <Suspense>
    <div>
      <AsyncCityView />
    </div>
    <template>
      <p>loading...</p>
    </template>
  </Suspense>
</template>

<script setup>
import AsyncCityView from '../components/AsyncCityView.vue';


</script>
