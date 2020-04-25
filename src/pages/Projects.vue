<template>
    <Layout>
        <div class="projects-page">
            <projects-banner />
        </div>
    </Layout>
</template>

<script>
import ProjectsBanner from "../components/Projects/ProjectsBanner";
import Projects from '../constants/projects.json';

export default {
    data: () => ({
        projects: Projects
    }),
    components: {
        ProjectsBanner,
    },
    metaInfo: {
        title: 'Projects'
    }
}
</script>

<style scoped>
    .projects-page {
        flex: 1;
    }
</style>
