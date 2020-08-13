<template>
  <main>
    <h1>Poker Planning</h1>
    <GoogleLoginButton @click="goAuth" />
  </main>
</template>

<script lang="ts">
import { Vue, Component } from 'vue-property-decorator'
import { Auth } from '@nuxtjs/auth'
import GoogleLoginButton from '../components/google-login-button.vue'

@Component
export default class LoginComponent extends Vue {
  readonly auth = 'guest'
  readonly $auth: Auth

  components = {
    GoogleLoginButton
  }

  goAuth () {
    this.$auth.loginWith('google')
  }
}
</script>

<style scoped>
main {
  display: inline-flex;
  flex-direction: column;
  justify-content: center;
}

h1 {
  text-align: center;
  margin-block-end: 1.5em;
}
</style>
