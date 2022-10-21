<template>
  <div class="w-full form-group">
    <input
      type="email"
      class="flex px-3 pt-2 border border-blue-200 rounded bg-blue-50 w-100 focus:outline-none focus:border-teal-800 h-11 w-96"
      :placeholder="placeholder"
    />
  </div>
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
