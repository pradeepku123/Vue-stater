<template>
  <h1>hiii {{ name }}</h1>
  <div v-text="comp"></div>
  <div v-html="channel"></div>
  <div v-bind:id="testID">VBind</div>
  <button :disabled="isDisabled">Submit</button>
  <div class="testClass">TEST</div>
  <div :class="status">TEST-001</div>
  <div :class="isPromoted && 'testClass'">TEST-002</div>
  <div :class="isPromoted && 'testClass'">TEST-003</div>
  <div :class="['sucess', 'testClass']">TEST-004</div>
  <div
    :class="[isPromoted && 'testClass', isPromoted ? 'sucess' : 'testClass']"
  >
    TEST-005
  </div>
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
      status: "sucess",
      isPromoted: true,
      isTrue: false,
    };
  },
};
</script>

<style>
* {
  background: rgb(207, 167, 167);
  text-align: center;
}
.testClass {
  background: rgb(162, 24, 24);
  text-align: center;
}
.sucess {
  background: rgb(201, 210, 201);
  text-align: center;
}
</style>
