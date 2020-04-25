<template>
    <div class="project-card">
        <div class="project-title">{{title}}</div>
        <div class="content-wrapper">
            <div class="project-description">{{description}}</div>
            <div v-if="showDetails" class="project-details">
                <span>{{starCount}} <font-awesome :icon="['fas', 'star']" class="star-icon" /></span>
                <span><font-awesome :icon="['fas', 'circle']" :style="{color: languageColor}" /> {{primaryLanguage}}</span>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        title: String,
        description: String,
        showDetails: Boolean,
        starCount: Number,
        primaryLanguage: String,
        languageColor: String
    }
}
</script>

<style scoped>
    .project-card {
        flex: 1;
        background: #F4F4F4;
        margin: 0 2rem;
        padding: 1rem;
        display: flex;
        flex-direction: column;
        min-height: 150px;
    }
    .project-card:first-child,
    .project-card:last-child {
        margin: 0
    }

    .project-title {
        font-size: 1.2rem;
        font-weight: 500;
        margin-bottom: 0.8rem;
    }

    .content-wrapper {
        flex: 1;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
    }

    .project-details {
        margin-top: 1rem;
        display: flex;
        justify-content: space-between;
    }
</style>