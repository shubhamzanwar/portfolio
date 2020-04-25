<template>
  <div class="display-row">
    <div class="title">{{title}}</div>
    <div class="content-wrapper">
        <slot>content</slot>
    </div>
    <div class="view-more">
        <g-link :to="viewMoreLink" class="view-more-link">
            {{viewMoreText}} <font-awesome :icon="['fas', 'long-arrow-alt-right']" />
        </g-link>
    </div>
  </div>
</template>

<script>
export default {
    props: {
        title: String,
        viewMoreText: String,
        viewMoreLink: String,
    }
}
</script>

<style scoped>
    .display-row {
        margin-top: 2rem;
    }

    .title {
        font-weight: 500;
        font-size: 2rem;
    }

    .content-wrapper {
        padding: 2rem 0;
    }

    .view-more {
        display: flex;
        justify-content: flex-end;
    }

    .view-more-link {
        text-decoration: none;
        color: #000;
    }

</style>