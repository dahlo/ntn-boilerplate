<template>
  <main>
    <section class="self-center flex flex-col flex-1 items-center justify-center">
      <h1 class="title text-center">NBIS</h1>
      <h2 class="subtitle text-center">National Bioinformatic Infrastructure Sweden</h2>
    </section>

    <section class="mt-4">
      <h3 class="text-primary-600 dark:text-primary-400 max-w-5xl mx-auto">Latest news</h3>
      <posts post-type="blog" :amount="5" />
    </section>
    <section class="mt-4">
      <h3 class="text-primary-600 dark:text-primary-400 max-w-5xl mx-auto">Events</h3>
      <posts post-type="blog" :amount="5" />
    </section>
  </main>
</template>
