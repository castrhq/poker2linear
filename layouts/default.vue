<template>
  <Nuxt />
</template>

<style>
* {
  margin: 0;
  padding: 0;
}

html {
  color: var(--foreground);
  font-family:
    'fira sans light',
    sans-serif;

  font-weight: 200;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

:root {
  --background: #08193E;
  --foreground: #F7F7F7;
}

body {
  height: 100vh;
  width: 100vw;

  background-image: url('~assets/img/cards-background.svg'),
    linear-gradient(to right, rgb(8, 25, 62), rgb(8, 25, 62));
  background-repeat: no-repeat, repeat;
  background-position: 25vw 50vh, center center;
}

@media (min-width: 640px) {
  body {
    background-position: 50vw 50vh, center center;
  }
}

@media (min-width: 1024px) {
  body {
    background-position: 75vw 50vh, center center;
  }
}

#__nuxt {
  display: flex;
  align-items: center;
  justify-content: center;

  height: 100%;
  width: 100%;
}

#__layout {
  display: flex;
  align-items: center;
  justify-content: center;

  height: 100%;
  width: 100%;
}
</style>
