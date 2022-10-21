<template>
  <input
    type="text"
    class="px-4 border border-blue-200 rounded bg-blue-50 w-44 focus:outline-none focus:border-teal-800 h-11"
  />
</template>

<script>
export default {
  props: {
    placeholder: {
      default: "",
    },
  },
};
</script>
