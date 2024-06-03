<template>
  <div class="bg-gray-100 grid lg:grid-cols-2 2xl:grid-cols-5">
    <div
      class="px-8 py-12 max-w-md mx-auto sm:max-w-xl lg:px-12 lg:py-24 lg:max-w-full xl:mr-0 2xl:col-span-2"
    >
      <div class="xl:max-w-xl">
        <img src="../assets/logo-brand.svg" class="h-10" />
        <img
          src="../assets/beach-work.jpg"
          class="mt-6 rounded-lg shadow-xl sm:mt-8 sm:h-64 sm:w-full sm:object-cover object-center lg:hidden"
        />
        <h1
          class="text-2xl font-bold text-gray-900 transition-all selection:text-brand sm:mt-8 lg:text-3xl xl:text-4xl"
        >
          You can work from anywhere.<br />
          <span class="text-brand selection:text-gray-800"
            >Take advantage of it.</span
          >
        </h1>
        <p class="mt-2 text-gray-600 sm:mt-4 sm:text-xl">
          Workcation helps you find work-frindly rentals in beautiful location
          so you can enjoy time some nice weather even when you aren't on
          vaction.
        </p>
        <div class="sm:mt-6 text-white text-sm">
          <button class="btn">Book your escape</button>
        </div>
      </div>
    </div>
    <div class="hidden relative lg:block 2xl:col-span-3">
      <img
        class="absolute inset-0 w-full h-full object-cover object-center"
        src="../assets/beach-work.jpg"
        alt="Woman workcationing on the beach"
      />
    </div>
  </div>
</template>
