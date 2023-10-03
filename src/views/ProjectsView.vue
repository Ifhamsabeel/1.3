<template>
  <div class="projects">
    <h1>Projects</h1>
    <ProjectCard
      v-for="project in projects"
      :key="project.id"
      :title="project.title"
      :description="project.description"
      :detailsLink="project.detailsLink"
    />
  </div>
</template>

<script>
import ProjectCard from '@/components/ProjectCard.vue'

export default {
  components: {
    ProjectCard
  },
  data() {
    return {
      projects: [
        {
          id: 1,
          title: 'Project 1',
          description: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit.',
          detailsLink: '#'
        },
        {
          id: 2,
          title: 'Project 2',
          description: 'Ut eget arcu vel tortor dignissim hendrerit.',
          detailsLink: '#'
        },
        {
          id: 3,
          title: 'Project 3',
          description: 'Integer euismod magna at tortor maximus vestibulum.',
          detailsLink: '#'
        }
      ]
    }
  }
}
</script>

<style scoped>
.projects {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 20px;
}

.projects h1 {
  font-size: 1.5rem;
}

@media (min-width: 768px) {
  .projects {
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: space-between;
  }
}

@media (min-width: 1024px) {
  .projects {
    min-height: 100vh;
  }
}
</style>
