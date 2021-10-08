<template>
  <main>
    <section v-if="posts" class="w-full max-w-5xl mx-auto">
      <h1 class="title">Support</h1>
      <posts post-type="support" :amount="10" />
    </section>
  </main>
</template>

<script>
export default {
  async asyncData({ $content, error }) {
    let posts;
    try {
      posts = await $content("support").fetch();
    } catch (e) {
      error({ message: "Pages not found" });
    }
    return { posts };
  },
}
</script>
