<script setup>
import { onMounted, ref } from "vue";
import DestinationServices from "../services/DestinationServices";
import DestinationsCard from "./DestinationsCard.vue";

const destinations = ref([]);

onMounted(() => {
  DestinationServices.getDestinations()
    .then((response) => (destinations.value = response.data))
    .catch((err) => console.error(err));
});
</script>

<template>
  <div class="max-w-md mx-auto py-8 sm:max-w-xl lg:max-w-screen-xl lg:px-12">
    <div>
      <h2 class="text-gray-800 text-xl font-semibold">Popular destinations</h2>
      <p class="text-gray-600 mt-4">
        A selection of great work-friendly cities with lots to see and explore.
      </p>
    </div>
    <div class="mt-6 grid gap-6 lg:grid-cols-2 xl:grid-cols-3">
      <DestinationsCard
        v-for="(destination, index) in destinations"
        :key="index"
        :destination="destination"
      />
    </div>
  </div>
</template>
