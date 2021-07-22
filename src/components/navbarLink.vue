<template>
  <div class="navbar-link-container">
    <router-link class="navbar-link" :to="link.path">
      {{ link.name }}
    </router-link>
  </div>
</template>

<script>
export default {
  props: {
    link: {
      required: true,
      type: Object,
    },
  },
};
</script>

<style>
</style>