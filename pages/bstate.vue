<template>
  <div>
    <NavBar></NavBar>
    <card>
      <div class="ml-44">
        <div class="justify-between mt-32 font-bold px-96 text-[#080A3C]">
          <h2>Business State</h2>
        </div>
        <div class="justify-between text-xs font-bold text-gray-400 px-96">
          <h3>From the below list, select what fits you best</h3>
        </div>
        <RadioBtn1></RadioBtn1>
        <RadioBtn2></RadioBtn2>
        <RadioBrn3></RadioBrn3>
      </div>
      <div class="flex justify-center mr-8">
        <NextBtn></NextBtn>
      </div>
    </card>
  </div>
</template>

<script>
import NavBar from "../components/container/NavBar.vue";
import NextBtn from "../components/buttons/NextBtn.vue";
import RadioBtn1 from "../components/buttons/RadioBtn1.vue";
import RadioBtn2 from "../components/buttons/RadioBtn1.vue";
import RadioBtn3 from "../components/buttons/RadioBtn3.vue";

export default {
  components: {
    NavBar,
    NextBtn,
    RadioBtn1,
    RadioBtn2,
    RadioBtn3,
  },
};
</script>
