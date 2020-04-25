<template>
  <Layout>
    <div class="home-page">
      <home-banner></home-banner>
    </div>
  </Layout>
</template>

<script>
import HomeBanner from "../components/HomeBanner";

export default {
  metaInfo: {
    title: 'Hello'
  },
  components: {
    HomeBanner: HomeBanner
  }
}
</script>

<style scoped>
  .home-page {
    flex: 1;
  }

</style>
