<template>
  <main />
</template>

<script lang="ts">
import { Vue, Component } from 'vue-property-decorator'

@Component
export default class IndexComponent extends Vue {
  created () {
    if (this.$store.state?.teams?.id === undefined) {
      this.$router.push('/teams/find')
    }
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
}
</style>
