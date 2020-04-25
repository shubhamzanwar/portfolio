<template>
    <Layout>
        <div class="blog-page">
            <projects-banner />
            <blog-alert />
            <projects-grid />
            <divider />
        </div>
    </Layout>
</template>

<script>
import ProjectsBanner from "../components/Projects/ProjectsBanner";
import BlogAlert from "../components/Blog/BlogAlert";
import ProjectsGrid from "../components/Projects/ProjectsGrid";
import Divider from "../components/Divider";
import Projects from '../constants/projects.json';

export default {
    data: () => ({
        projects: Projects
    }),
    components: {
        ProjectsBanner,
        BlogAlert,
        ProjectsGrid,
        Divider,
    },
    metaInfo: {
        title: 'Blog'
    }
}
</script>

<style scoped>
    .blog-page {
        flex: 1;
    }
</style>
