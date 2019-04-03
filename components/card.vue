<template>
  <section>
    <div class="fl w-100 ba pv4 ph3 br3 vh-50">
      <div class="fl w-100 lh-title f4 pt2 bb">{{field}}</div>
      <div class="fl w-100 lh-title f2 pv4">{{trend}}</div>
    </div>
  </section>
</template>

<script>
export default {
  props: ["field", "trend"]
};
</script>
