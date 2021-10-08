<template>
  <div class="wrapper">
    <NavBar />
    <nuxt />

    <div class="grid grid-flow-col gap-3">
      <section class="mt-4">
        <h3 class="text-primary-600 dark:text-primary-400 mx-auto">Latest news</h3>
        <posts post-type="blog" :amount="5" />
      </section>
      <section class="mt-4">
        <h3 class="text-primary-600 dark:text-primary-400 mx-auto">Events</h3>
        <posts post-type="blog" :amount="5" />
      </section>
    </div>

    <ColorModePicker />
  </div>
</template>
