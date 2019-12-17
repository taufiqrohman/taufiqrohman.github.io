<template>
  <a
    v-bind:href="link"
    :class="`inline-block text-${color}-800 bg-${color}-400 px-2 border border-${color}-600 rounded-sm mr-1`"
    target="_blank"
  >{{name}}</a>
</template>

<script>
export default {
  name: "Contact",
  props: {
    name: String,
    icon: String,
    link: String,
    color: {
      type: String,
      default: "green"
    }
  }
};
</script>