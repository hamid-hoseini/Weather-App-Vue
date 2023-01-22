14 lines (13 sloc)  253 Bytes

<template>
  <div>
    <Suspense>
      <AsyncCityView />
      <template #fallback>
        <CityViewSkeleton />
      </template>
    </Suspense>
  </div>
</template>
<script setup>
import AsyncCityView from '../components/AsyncCityView.vue';
import CityViewSkeleton from '../components/CityViewSkeleton.vue';


</script>
