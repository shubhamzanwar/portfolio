<template>
  <div class="base" :class="type">
      <slot></slot>
  </div>
</template>

<script>
export default {
    props: {
        type: String
    }
}
</script>

<style scoped>
    .base {
        padding: 1rem;
        font-size: 1.2rem;
        font-weight: 400;
        text-align: center;
        border-radius: 10px;
    }
    .info {
        background: #CCE5FF;
        border: 1px solid #B8DAFF;
        color: #004085;
    }
    .warning {
        background: #FFF3CD;
        border: 1px solid #FFEEBA;
        color: #856404;
    }
</style>