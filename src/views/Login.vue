<template>
  <div class="wrapper">
    <label class="darkMode">
      <input type="checkbox" class="nes-checkbox" checked />
      <span>Enable</span>
    </label>
    <Form />
  </div>
</template>

<script>
import Form from "../components/Form";
export default {
  name: "Login",
  components: {
    Form,
  },

  data: () => ({}),
  methods: {},
};
</script>
<style lang="scss">
* {
  box-sizing: border-box;
  font-family: "Press Start 2P";
}

.darkMode {
  position: absolute;
  right: 10px;
  top: 10px;
}
</style>
