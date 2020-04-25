<template>
  <Layout>
    <div class="home-page">
      <home-banner></home-banner>
      <intro-row></intro-row>
    </div>
  </Layout>
</template>

<script>
import HomeBanner from "../components/Home/HomeBanner";
import IntroRow from "../components/Home/IntroRow";

export default {
  metaInfo: {
    title: 'Hello'
  },
  components: {
    HomeBanner,
    IntroRow
  }
}
</script>

<style scoped>
  .home-page {
    flex: 1;
  }

</style>
