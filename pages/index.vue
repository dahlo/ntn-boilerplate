<template>
  <main>
    <nuxt-content :document="page" />
  </main>
</template>

<script>
export default {
  layout: 'index',
  async asyncData ({ $content }) {
    const page = await $content('index').fetch()
    return {
      { page }
    }
  }
}
</script>
