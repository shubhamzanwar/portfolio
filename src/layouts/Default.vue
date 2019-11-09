<template>
  <div class="layout">
    <header class="header">
      <strong>
        <g-link v-show="showBrand" to="/" class="brand-btn">SZ</g-link>
      </strong>
      <nav class="nav">
        <g-link class="nav__link" to="/about">About</g-link>
        <g-link class="nav__link" to="/projects">Projects</g-link>
        <g-link class="nav__link" to="/contact">Contact</g-link>
      </nav>
    </header>
    <slot/>
  </div>
</template>

<style>
  body {
    font-family: 'Avenir', -apple-system,system-ui,BlinkMacSystemFont,"Segoe UI",Roboto,"Helvetica Neue",Arial,sans-serif;
    margin: 0;
    padding: 0;
    line-height: 1.5;
  }

  .layout {
    margin: 0 auto;
    padding: 0 1.25rem;
    border: 2rem solid black;
    height: 100vh;
    box-sizing: border-box;
    display: flex;
    flex-direction: column;
  }

  .header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 1.25rem;
    height: 1.75rem;
    margin-top: 1rem;
  }

  .brand-btn {
    text-decoration: none;
    font-size: 1.75rem;
    color: black;
  }

  .nav__link {
    text-decoration: none;
    font-size: 1.25rem;
    color: black;
    margin-left: 1.25rem;
  }

  @media only screen and (max-width: 768px) {
    .layout {
      border: none;
    }
  }
</style>

<script>
export default {
  data: () => ({
    showBrand: false
  }),
  mounted() {
    this.showBrand = this.$route.fullPath !== "/";
  }
}
</script>
