<template>
  <input
    type="tel"
    class="px-3 border border-blue-200 rounded bg-blue-50 focus:outline-none focus:border-teal-800 h-11 w-96"
    :placeholder="placeholder"
  />
</template>

<script>
export default {
  props: {
    placeholder: {
      type: String,
      default: "",
    },
  },
};
</script>
