<template>
  <v-app id="wrapper">
    <div class="darkMode">
      <label>
        <input type="checkbox" class="nes-checkbox" />
        <span>Dark Mode</span>
      </label>
    </div>
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
      <router-link to="/game">asd</router-link>
    </div>
    <router-view></router-view>
  </v-app>
</template>

<script>
export default {
  name: "App",

  components: {},
  props: ["nick"],

  data: () => ({
    nick: "",
  }),
};
</script>
<style>
* {
  box-sizing: border-box;
  font-family: "Press Start 2P";
}
.darkMode {
  position: absolute;
  right: 10px;
  top: 10px;
}

.form {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  border: 1px solid #000;
  padding: 10px;
  width: 80%;
}
</style>
