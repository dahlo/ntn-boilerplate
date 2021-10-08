<template>
  <div class="wrapper">
    <NavBar />
    <nuxt />

    <section class="mt-4">
      <h3 class="text-primary-600 dark:text-primary-400 max-w-1/2 mx-auto">Latest news</h3>
      <posts post-type="blog" :amount="5" />
    </section>
    <section class="mt-4">
      <h3 class="text-primary-600 dark:text-primary-400 max-w-1/2 mx-auto">Events</h3>
      <posts post-type="blog" :amount="5" />
    </section>

    <ColorModePicker />
  </div>
</template>
