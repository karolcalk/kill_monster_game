<template>
  <div class="form">
    <div class="nes-field">
      <label for="name_field">Your name</label>
      <input type="text" id="name_field" class="nes-input" />
    </div>
    <div class="nes-field">
      <label for="name_field">email</label>
      <input type="text" id="name_field" class="nes-input" />
    </div>
    <div class="nes-field">
      <label for="name_field">Your nick</label>
      <input type="text" id="name_field" class="nes-input" v-model="nick" />
    </div>

    <router-link to="/game"
      ><button type="button" class="nes-btn is-primary">Primary</button>
    </router-link>
  </div>
</template>

<script>
export default {
  name: "Form",
};
</script>

<style lang="scss">
.form {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  border: 1px solid rgb(143, 100, 100);
  padding: 10px;
  width: 80%;
}
</style>
