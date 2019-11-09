<template>
  <Layout>
    <div class="home-page">
      <div class="name-block">
      </div>
      <div class="name">Shubham <br> Zanwar</div>
    </div>
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'Hello'
  }
}
</script>

<style scoped>
  .home-page {
    flex: 1;
    position: relative;
  }

  .name-block {
    position: absolute;
    bottom: 8rem;
    left: 6rem;
    background: #B0F3D7;
    height: 50vh;
    width: 40vw;
  }

  .name {
    position: absolute;
    bottom: 8rem;
    left: 7rem;
    font-size: 5.6rem;
    font-weight: bold;
  }

  @media only screen and (max-width: 768px) {
    .name-block {
      bottom: 3rem;
      left: 0;
      height: 24rem;
      width: 100%;
    }
    .name {
      bottom: 3rem;
      left: 1rem;
      font-size: 4rem;
    }
  }
</style>
