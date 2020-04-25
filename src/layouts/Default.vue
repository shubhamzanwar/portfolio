<template>
  <div class="layout">
    <header class="header">
      <strong>
        <g-link to="/" class="brand-btn">SZ</g-link>
      </strong>
    </header>
    <slot/>
    <footer class="footer">
      © Shubham Zanwar
    </footer>
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
    padding: 0 2rem;
    max-width: 1280px;
    width: 100%;
    height: 100vh;
    box-sizing: border-box;
    display: flex;
    flex-direction: column;
    overflow: auto;
  }

  .header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 1.25rem;
    height: 1.75rem;
    margin-top: 3rem;
  }

  .footer {
    padding-bottom: 3rem;
    font-size: 0.8rem;
    color: #999999;
  }

  .brand-btn {
    text-decoration: none;
    font-size: 1.75rem;
    font-weight: normal;
    color: black;
  }
</style>

<script>
export default {
}
</script>
