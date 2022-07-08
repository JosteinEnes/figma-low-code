<template>
  <div class="home">
    <Figma :figma="figmaConfig" v-model="viewModel" :config="config"/>
  </div>
</template>

<script>
// https://github.com/KlausSchaefers/figma-low-code code found here


import Vue from "vue";
import Figma from "vue-low-code";
Vue.use(Figma);

// import JSON file for deployment 
// import app from './app.json'

/* The code for using app.json instead of getting the view from the figma.com. You also need to add the FigmaJSON: in the return

<template>
  <div class="home">
    <Luisa :design="figmaJSON" v-model="viewModel" :config="config"/>
  </div>
</template>


<script>
import Vue from "vue";
import Luisa from "luisa-vue";
Vue.use(Luisa);
*/

export default {
  name: "Home",
  data: function () {
    return {
      // figmaJSON: app  //add to use the file instead of web
      figmaConfig: {
        figmaFile: "9k8JIDGZXUNNYrEn501zmH",
        figmaAccessKey: "figd_C88fba7jcWWMujeTOtV5YcBrWzFyYJ8nJlH3qIAb",
      },
      viewModel: {
        /**
         * Add your view model here
         */
      },
      config: {
 /*       responsive: [
          { value: "Desktop", label: "Desktop", types: ["desktop"] },
          { value: "Mobile", label: "Mobile", types: ["tablet", "mobile"] },
        ], 
        */
        components: {
          /**
           * Register costum components here
           */
        },
      },
    };
  },
  components: {},
  methods: {
    /**
     * Place your methods here
     */
  },
};
</script>
