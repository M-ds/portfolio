<template>
  <v-app>
    <v-main>
      <v-container>
        <welcome/>
        <hr>
        <skills/>
        <hr>
        <work-experience/>
      </v-container>
    </v-main>
    <hr>
    <v-footer absolute>
      Made by Michiel with Vuetify
    </v-footer>
  </v-app>
</template>

<script lang="ts" setup>
import Welcome from "@/components/welcome/Welcome.vue";
import WorkExperience from "@/components/work/WorkExperience.vue";
import Skills from "@/components/skills/Skills.vue";
</script>
