<template>
  <div @click="goAuth">
    <img class="logo" alt="Google" src="~/assets/img/google-icon.svg">
    <p>Sign in with Google</p>
  </div>
</template>

<script lang="ts">
import { Component, Emit, Vue } from 'vue-property-decorator'

@Component
export default class GoogleLoginButtonComponent extends Vue {
  @Emit('click')
  goAuth () {}
}
</script>

<style scoped>
div {
  display: inline-flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;

  cursor: pointer;
  background-color: white;

  box-sizing: border-box;
  border-radius: 4px;

  padding: 1.125em;
  font-size: 0.875em;

  box-shadow: 0 2px 4px rgba(0,0,0,0.25);
}

div:active {
  background-color: #EEEEEE;
}

img.logo {
  height: 2.25em;
  margin-right: 1.125em;
}

p {
  font-family: 'Roboto Medium';
  font-size: 1.5em;
  line-height: 1.5em;

  color: #757575;
}
</style>
