<template>
    <banner
        title="Hi, I'm Shubham Zanwar"
        subTitle="A full stack software development engineer"
    >
        <template v-slot:image>
            <g-image src="~/assets/home.png" class="banner-image" />
        </template>
    </banner>
</template>

<script>
import Banner from "../Banner";

export default {
  components: {
    banner: Banner
  }
}
</script>

<style>
  .banner-image {
    width: 26rem;
  }
</style>