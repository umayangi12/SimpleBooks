<template>
  <center>
    <NavBar></NavBar>
    <div class="max-w-3xl px-4 mx-auto mb-3 my-25">
      <SignUpContainer>
        <div class="flex space-x-4">
          <div>
            <label for="firstName">First Name</label>
            <NameInput></NameInput>
          </div>

          <div>
            <label for="firstName">Last Name</label>
            <NameInput></NameInput>
          </div>
        </div>

        <label for="email">Email Address</label>
        <EmailInput
          class="mt-2 text-secondary"
          placeholder="example@gmail.com"
        ></EmailInput>

        <label for="phoneNumber">Phone Number</label>
        <PNInput
          class="mt-2 text-secondary"
          placeholder="00 00 00 000"
        ></PNInput>

        <div class="form-group">
          <label for="password">Password</label>
          <PasswordInput class="mt-2 text-secondary"></PasswordInput>
        </div>
        <div class="gap-y-4">
          <SubmitBtn></SubmitBtn>
          <br />
          <div class="inline-flex items-center justify-center w-full">
            <hr class="h-px my-8 bg-gray-400 border-0 w-96" />
            <span
              class="absolute px-3 font-sans font-medium text-gray-500 -translate-x-1/2 bg-white left-1/2 dark:text-gray-600"
              >Or</span
            >
          </div>
          <GoogleBtn></GoogleBtn>
        </div>
        <div class="flex items-center justify-center mt-4 ml-24">
          <p>
            Already have an account?
            <a
              class="cursor-pointer  hover:text-sky-400 hover:underline text-[#3C5CCF]"
              @click="goto"
              >Sign in</a
            >
          </p>
        </div>
      </SignUpContainer>
    </div>
  </center>
</template>

<script>
import NameInput from "../../components/inputs/NameInput.vue";
import SignUpContainer from "../../components/container/SignUpContainer.vue";
import EmailInput from "../../components/inputs/EmailInput.vue";
import PNInput from "../../components/inputs/PNInput.vue";
import PasswordInput from "../../components/inputs/PasswordInput.vue";
import GoogleBtn from "../../components/buttons/GoogleBtn.vue";
import SubmitBtn from "../../components/buttons/SubmitBtn.vue";
import NavBar from "../../components/container/NavBar.vue";

export default {
  components: {
    NameInput,
    SignUpContainer,
    EmailInput,
    PNInput,
    PasswordInput,
    GoogleBtn,
    SubmitBtn,
    NavBar,
  },
  methods: {
    goto() {
      this.$router.push("/login");
    },
  },
};
</script>

<style>
.signup-panel {
  padding: 200px;
}

.display-3 {
  font-family: calibri;
  font-size: 40px;
}

.input-label {
  padding: 0px;
}

.form-control {
  block-size: 30px;
  border-radius: 6px;
  width: 400px;
}
</style>
