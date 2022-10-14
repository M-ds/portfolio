<script setup lang="ts">
import { ref } from "vue";

const menuOpen = ref(false);
</script>

<template>
  <div id="side_menu">
    <button
      class="side_menu__btn"
      @click="menuOpen = !menuOpen"
      :class="{ active: menuOpen }"
    >
      <span class="top"></span>
      <span class="mid"></span>
      <span class="bottom"></span>
    </button>
    <Transition name="fade">
      <nav v-if="menuOpen">
        <router-link class="box" to="/">Home</router-link>
        <router-link class="box" to="/about">About</router-link>
        <router-link class="box" to="/work">Work</router-link>
      </nav>
    </Transition>
  </div>
</template>
