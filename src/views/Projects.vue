<template>
  <div  class="home">
      <ProjectsComponent />
  </div>
</template>

<script>
// @ is an alias to /src
import ProjectsComponent from "@/components/ProjectsComponent.vue";

export default {
  name: 'Projects',
  components: {
    ProjectsComponent
  }
};
</script>

<style>
</style>
