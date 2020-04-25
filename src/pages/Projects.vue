<template>
    <Layout>
        <div class="projects-page">
            <projects-banner />
            <projects-alert />
        </div>
    </Layout>
</template>

<script>
import ProjectsBanner from "../components/Projects/ProjectsBanner";
import ProjectsAlert from "../components/Projects/ProjectsAlert";
import Projects from '../constants/projects.json';

export default {
    data: () => ({
        projects: Projects
    }),
    components: {
        ProjectsBanner,
        ProjectsAlert,
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
