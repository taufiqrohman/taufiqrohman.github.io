<template>
  <div
    :class="`inline-block bg-${color}-400 rounded-sm border border-${color}-600 py-2 p-4 mr-1 text-${color}-900 font-bold`"
  >{{ title }}</div>
</template>

<script>
export default {
  name: "Skill",
  props: {
    title: String,
    level: Number,
    color: {
      type: String,
      default: "blue"
    }
  }
};
</script>