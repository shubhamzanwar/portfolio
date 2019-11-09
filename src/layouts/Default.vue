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
    padding-left: 20px;
    padding-right: 20px;
    border: 32px solid black;
    height: 100vh;
    box-sizing: border-box;
  }

  .header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
    height: 28px;
    margin-top: 14px;
  }

  .brand-btn {
    text-decoration: none;
    font-size: 28px;
    color: black;
  }

  .nav__link {
    margin-left: 20px;
    text-decoration: none;
    color: black;
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
