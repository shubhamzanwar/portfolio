<template>
  <Layout>
    <div class="home-page">
      <home-banner />
      <intro-row />
      <divider />
    </div>
  </Layout>
</template>

<script>
import HomeBanner from "../components/Home/HomeBanner";
import IntroRow from "../components/Home/IntroRow";
import Divider from "../components/Divider";

export default {
  metaInfo: {
    title: 'Hello'
  },
  components: {
    HomeBanner,
    IntroRow,
    Divider
  }
}
</script>

<style scoped>
  .home-page {
    flex: 1;
  }

</style>
