<template>
  <main class="ui container">
    <div class="ui three stackable cards">
      <Card v-for="(project, i) in $appData.projects"
            :key="i"
            :name="project.name"
            :imageSource="project.image"
            :date="project.date"
            :description="project.description"
            :meta="project.meta"
      ></Card>
    </div>
  </main>
</template>
<script>
  import Card from './components/ProjectCard.vue';

  export default {
    components: {
      Card
    }

  }
</script>
