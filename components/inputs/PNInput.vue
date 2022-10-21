<template>

   <input
          type="tel"
          class="w-full px-4 py-1 bg-blue-100 border border-blue-200 rounded focus:outline-none focus:border-teal-800"
          :placeholder="placeholder"
        />
       

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