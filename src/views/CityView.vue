14 lines (13 sloc)  253 Bytes

<template>
  <div>
    <Suspense>
      <AsyncCityView />
      <template #fallback>
        <p>Loading...</p>
      </template>
    </Suspense>
  </div>
</template>
<script setup>
import AsyncCityView from '../components/AsyncCityView.vue';


</script>
