<template>
  <center>
     <NavBar></NavBar>
    <div class ="max-w-3xl px-4 mx-auto mb-3 my-25 ">
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
        <PNInput class="mt-2 text-secondary"></PNInput>

   
        <div class="form-group">
          <label for="password">Password</label>
          <PasswordInput class="mt-2 text-secondary"></PasswordInput>
        </div>
        <br />
        <br />
        <br />
        <div class="gap-y-4">
          <SubmitBtn></SubmitBtn>
          <br />
          <div class="mt-4 bg-white rounded-lg shadow-md">
            <div class="h-1 bg-gray-400 rounded-t-md"></div>
          </div>
          <br />
          <GoogleBtn></GoogleBtn>
        </div>
        <br/>
        <br/>
        <div class="flex items-center justify-center">
          <p>Already have an account? <a class="text-blue-700 hover:text-sky-400 hover:underline"  href="">Sign in</a></p>
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
import NavBar from "../../components/container/NavBar.vue"
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
