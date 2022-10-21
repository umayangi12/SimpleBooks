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
        <div class="flex items-center mt-4 mb-4 px-96">
          <input
            id="default-radio-1"
            type="radio"
            value=""
            name="default-radio"
            class="w-4 h-4 bg-gray-100 border-gray-300 dark:ring-offset-gray-800 focus:ring-2 dark:bg-gray-700 dark:border-gray-600"
          />
          <label
            for="default-radio-1"
            class="ml-2 text-sm font-bold text-gray-900 dark:text-gray-900"
            >I want to incorporate my business with Simplebooks</label
          >
        </div>
        <div class="flex items-center mb-4 px-96">
          <input
            checked
            id="default-radio-2"
            type="radio"
            value=""
            name="default-radio"
            class="w-4 h-4 bg-gray-100 border-gray-300 dark:ring-offset-gray-800 focus:ring-2 dark:bg-gray-700 dark:border-gray-600"
          />
          <label
            for="default-radio-2"
            class="ml-2 text-sm font-bold text-gray-900 dark:text-gray-900"
            >My business is already incorparated</label
          >
        </div>
        <div class="flex items-center mb-4 px-96">
          <input
            checked
            id="default-radio-3"
            type="radio"
            value=""
            name="default-radio"
            class="w-4 h-4 bg-gray-100 border-gray-300 dark:ring-offset-gray-800 focus:ring-2 dark:bg-gray-700 dark:border-gray-600"
          />
          <label
            for="default-radio-3"
            class="ml-2 text-sm font-bold text-gray-900 dark:text-gray-900"
            >I am not looking to incorporate my business</label
          >
        </div>
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

export default {
  components: {
    NavBar,
    NextBtn,
   
  },
};
</script>
