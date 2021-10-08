<template>
  <div class="wrapper">
    <NavBar />
    <nuxt />

    <section class="flex flex-row">
      <h3 class="text-primary-600 dark:text-primary-400 mx-auto">Latest news</h3>
      <posts post-type="blog" :amount="5" />
      <h3 class="text-primary-600 dark:text-primary-400 mx-auto">Events</h3>
      <posts post-type="blog" :amount="5" />
    </section>

    <ColorModePicker />
  </div>
</template>
