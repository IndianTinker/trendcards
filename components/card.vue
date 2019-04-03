<template>
  <section>
    <div class="fl w-100 ba pa4 br3 vh-50">
      <div class="fl w-100 lh-title f3 pt2 bb">{{field}}</div>
      <div class="fl w-100 lh-title f1 pv4">{{trend}}</div>
    </div>
  </section>
</template>

<script>
export default {
  props: ["field", "trend"]
};
</script>
