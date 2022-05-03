<template>
  <section>
    <h2 class="section__title">{{ title }}</h2>
  </section>
</template>

<script setup>
import { defineProps } from "vue";
defineProps({
  title: String,
});
</script>
