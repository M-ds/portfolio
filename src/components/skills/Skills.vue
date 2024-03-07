<script setup lang="ts">

import SectionTitle from "@/components/common/SectionTitle.vue";
</script>

<template>
  <section-title :title="'Skills'"/>
  <v-row>
    <v-col>
      <v-list lines="one">
        <v-list-item
          v-for="n in 3"
          :key="n"
          :title="'Item ' + n"
          subtitle="Lorem ipsum dolor sit amet consectetur adipisicing elit"
        ></v-list-item>
      </v-list>
    </v-col>
    <v-col>
      <v-list lines="one">
        <v-list-item
          v-for="n in 3"
          :key="n"
          :title="'Item ' + n"
          subtitle="Lorem ipsum dolor sit amet consectetur adipisicing elit"
        ></v-list-item>
      </v-list>
    </v-col>
    <v-col>
      <v-list lines="one">
        <v-list-item
          v-for="n in 3"
          :key="n"
          :title="'Item ' + n"
          subtitle="Lorem ipsum dolor sit amet consectetur adipisicing elit"
        ></v-list-item>
      </v-list>
    </v-col>
  </v-row>
</template>

<style scoped>

</style>