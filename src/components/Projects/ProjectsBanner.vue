<template>
    <banner
        title="Hey there!"
        subTitle="Here is what I’ve been working on"
    >
        <template v-slot:image>
            <g-image src="~/assets/projects.png" class="banner-image" />
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