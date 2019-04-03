<template>
  <div class="mw9 w-100 pa4-ns pa4 ph5-ns system-sans-serif">
    <topbar message="About"/>
    <nuxt/>
  </div>
</template>

<script>
import topbar from "~/components/topbar.vue";
export default {
  components: {
    topbar
  }
};
</script>

