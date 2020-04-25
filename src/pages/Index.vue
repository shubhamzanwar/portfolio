<template>
  <Layout>
    <div class="home-page">
      <home-banner />
      <intro-row />
      <divider />
      <home-info-alert />
    </div>
  </Layout>
</template>

<script>
import HomeBanner from "../components/Home/HomeBanner";
import IntroRow from "../components/Home/IntroRow";
import Divider from "../components/Divider";
import HomeInfoAlert from "../components/Home/HomeInfoAlert";

export default {
  metaInfo: {
    title: 'Hello'
  },
  components: {
    HomeBanner,
    IntroRow,
    Divider,
    HomeInfoAlert
  }
}
</script>

<style scoped>
  .home-page {
    flex: 1;
  }

</style>
