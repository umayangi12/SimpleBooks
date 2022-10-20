<template>
  <div class="w-full form-group">
    <input
      type="email"
      class="w-full px-3 py-1 bg-blue-100 border border-blue-200 rounded w-100 focus:outline-none focus:border-teal-800"
      :placeholder="placeholder"
    />
  </div>
</template>

<script>
export default {
    props: {
        placeholder: {
            type: String,
            default:''
        }
    }
}
</script>
