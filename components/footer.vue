<template>
  <footer class="bg-info">
    <span class="text-white">©{{ actualYear }}</span>
    <div class="social">
      <font-awesome-icon :icon="['fab', 'facebook']" class="text-white"/>
      <font-awesome-icon :icon="['fab', 'instagram']" class="text-white"/>
      <font-awesome-icon :icon="['fab', 'twitter']" class="text-white"/>
      <font-awesome-icon :icon="['fab', 'linkedin']" class="text-white"/>
    </div>
  </footer>
</template>

<script>
export default {
  computed: {
    actualYear: () => new Date().getFullYear()
  }
}
</script>


<style scoped>
footer {
  display: flex;
  justify-content: space-around;
  align-items: center;
}
.social {
  font-size: 1.5em;
}
.social > * {
  cursor: pointer;
}
</style>
