<template>
  <main>
    <nuxt-content :document="page" />
  </main>
</template>

<script>
export default {
  layout: 'index',
  async asyncData ({ $content }) {
    let page;
    page = await $content('index').fetch()
    return {
      page
    }
  }
}
</script>
