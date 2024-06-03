<script setup>
const props = defineProps({
  destination: {
    type: Object,
    required: true,
  },
});
</script>

<template>
  <div
    class="flex items-center rounded-lg bg-white shadow-lg overflow-hidden max-h-32 hover:-translate-y-5 transform transition"
  >
    <div class="grid grid-cols-2">
      <img
        :src="destination.imageUrl"
        class="h-full object-cover object-center rounded-s-lg"
      />
      <div class="flex flex-col justify-center px-4">
        <h3 class="text-lg font-semibold text-gray-800">
          {{ destination.city }}
        </h3>
        <p class="text-gray-600">
          {{ destination.averagePrice }} / night average
        </p>
        <div class="mt-4">
          <a
            href="#"
            class="text-brand-dark hover:text-brand font-semibold text-sm"
            >Explore {{ destination.propertyCount }} properties</a
          >
        </div>
      </div>
    </div>
  </div>
</template>
