<template>
  <h1>hiii {{ name }}</h1>
  <div v-text="comp"></div>
  <div v-html="channel"></div>
  <div v-bind:id="testID">VBind</div>
  <button :disabled="isDisabled">Submit</button>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      name: "Pradeep",
      comp: "Delhi Chal1",
      channel: "<b>Hello World</b>",
      testID: "T001",
      isDisabled: true,
    };
  },
};
</script>

<style>
* {
  background: rgb(207, 167, 167);
  text-align: center;
}
</style>
