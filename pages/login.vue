<template>
  <div>
    <NavBar></NavBar>
    <div class="object-top my-25">
      <LoginContainer>
        <div class="px-24">
          <div class="ml-64 mr-4">
            <label for="email" class="">Email Address</label>
            <EmailInput
              class="mt-2 text-secondary"
              placeholder="example@gmail.com"
            ></EmailInput>

            <div class="mt-3 form-gtable-row-group">
              <label for="password">Password</label>
              <PasswordInput class="mt-2 text-secondary"></PasswordInput>
            </div>
            <SignInBtn @click="goto"></SignInBtn>
          </div>
        </div>
        <div class="flex justify-center mt-4">
          <p>
            Forgot Password?
            <a
              class="text-[#3C5CCF] cursor-pointer hover:text-sky-400 hover:underline"
              >Reset</a
            >
          </p>
        </div>
        <div class="inline-flex items-center justify-center w-full">
          <hr class="h-px my-8 bg-gray-400 border-0 w-96" />
          <span
            class="absolute px-3 font-sans font-medium text-gray-500 -translate-x-1/2 bg-white left-1/2 dark:text-gray-600"
            >Or</span
          >
        </div>
        <div class="flex justify-center mr-8"><GoogleBtn></GoogleBtn></div>
      </LoginContainer>
    </div>
  </div>
</template>

<script>
import NavBar from "../components/container/NavBar.vue";
import EmailInput from "../components/inputs/EmailInput.vue";
import PasswordInput from "../components/inputs/PasswordInput.vue";
import LoginContainer from "../components/container/LoginContainer.vue";
import SignInBtn from "../components/buttons/SignInBtn.vue";
import GoogleBtn from "../components/buttons/GoogleBtn.vue";

export default {
  components: {
    NavBar,
    EmailInput,
    PasswordInput,
    LoginContainer,
    SignInBtn,
    GoogleBtn,
  },
  methods: {
    goto() {
      this.$router.push("/bstate");
    },
  },
};
</script>
