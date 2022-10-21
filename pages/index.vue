<template>
  <sign-up />
</template>

<script>
import SignUp from "../components/signup/SignUp.vue";
import login from "../pages/login.vue";
export default {
  name: "IndexPage",
  components: {
    SignUp,
    login,
  },
};
</script>
