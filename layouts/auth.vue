<template>
  <div class="auth-page">
    <slot />
  </div>
</template>

<style lang="scss">
html {
  font-family: "Poppins", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto,
    Oxygen, Ubuntu, Cantarell, "Open Sans", "Helvetica Neue", sans-serif;
}
.auth-page {
  background-color: #000000;
  background-image: url("/assets/images/auth-background.svg");
  background-position: top right;
  background-repeat: no-repeat;
}
</style>
