<template>
    <div class="spacer">
        <alert type="info">
            All of these articles are available on 
            <a href="https://github.com/shubhamzanwar" target="_blank">medium</a>. I also soon play to start writing on
            <a href="https://dev.to/shubhamzanwar">Dev.to</a>.
        </alert>
    </div>
</template>

<script>
import Alert from "../Alert";

export default {
    components: {
        Alert
    }
}
</script>

<style scoped>
    .spacer {
        margin-top: 3rem;
    }
    a {
        color: inherit
    }
</style>