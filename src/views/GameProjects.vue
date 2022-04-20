<template>
  <div>
    <h1>Steam Games</h1>

    <div style="margin-bottom: 30px;">
      The following are Steam Games I've made or heavily contributed to.
    </div>

    <ProjectsList v-bind:projects="projects" />

    <div style="margin-top: 20px;">
      Explore my entire catalog of Steam Games <a target="_blank" href="https://store.steampowered.com/curator/37383610">here.</a>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import ProjectsList from "@/components/ProjectsList.vue";
import gameProjectsData from "@/data/GameProjectsData.ts";

export default Vue.extend({
  name: "GameProjects",
  components: {
    ProjectsList,
  },
  data: function () {
    return {
      projects: gameProjectsData,
    };
  },
});
</script>
