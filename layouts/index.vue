<template>
  <div class="wrapper">
  <div class="container mx-auto">
    <NavBar />
    <nuxt />

    <div class="container mx-auto">
      <div class="grid grid-cols-1 md:grid-cols-2">
        <div class="flex justify-center border-2 border-gray-300 rounded-xl p-6 bg-gray-100">
          <section class="mt-4">
            <h3 class="text-primary-600 dark:text-primary-400 mx-auto">Latest news</h3>
            <posts post-type="blog" :amount="5" />
          </section>
        </div>
        <div class="flex justify-center border-2 border-gray-300 rounded-xl p-6 bg-gray-100">
          <section class="mt-4">
            <h3 class="text-primary-600 dark:text-primary-400 mx-auto">Events</h3>
            <posts post-type="blog" :amount="5" />
          </section>
        </div>
      </div>

    <ColorModePicker />
  </div>
</template>
