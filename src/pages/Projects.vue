<template>
    <Layout>
        <div class="projects-page">
        <h2>Projects</h2>
        <div class="projects-grid">
            <a
                v-for="project in projects"
                :key="project.id"
                :href="project.url"
                class="project-container"
                target="_blank"
            >
                <div class="project">
                    <div>
                        <h5>{{project.name}}</h5>
                        <p>{{project.description}}</p>
                    </div>
                    <div class="project-details">
                        <span>
                            {{project.stargazers}} <font-awesome :icon="['fas', 'star']" class="star-icon" />
                        </span>
                        <span>
                            <font-awesome :icon="['fas', 'circle']" :style="{color: project.primaryLanguage.color}" />
                            {{project.primaryLanguage.name}}
                        </span>
                    </div>
                </div>
            </a>
        </div>
        </div>
    </Layout>
</template>

<script>
import Projects from '../constants/projects.json';

export default {
    data: () => ({
        projects: Projects
    }),
    metaInfo: {
        title: 'Hello'
    }
}
</script>

<style scoped>
    .projects-page {
        padding: 2rem;
    }

    .projects-grid {
        display: grid;
        grid-template-columns: 1fr 1fr 1fr 1fr;
        gap: 2rem;
    }

    .project-container {
        text-align: center;
        text-decoration: none;
        color: black;
        box-shadow: 0 0 10px #B0F3D7;
    }

    .project-container:hover {
        box-shadow: 0 0 20px #B0F3D7;
    }

    .project {
        min-height: 12rem;
        display: flex;
        flex-direction: column;
        justify-content: space-around;
    }

    .project-details {
        display: flex;
        justify-content: space-around
    }
</style>
