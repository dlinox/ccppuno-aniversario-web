<template>
  <header class="app-header">
    <div class="container">
      <img class="header-logo" src="~assets/images/logo-white.png" alt="" />
      <nav>
        <button class="btn btn-primary ">conseguir entradas </button>
      </nav>
    </div>
  </header>
</template>
<script setup></script>
<style scoped lang="scss">
.app-header {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;

  background-color: rgba($color: #000000, $alpha: 0.6);
  z-index: 2;
  padding: 1em 0;

  .container {
    display: flex;
    align-items: center;
    justify-content: space-between;

    .header-logo {
      height: 100%;
      width: 12em;
    }
  }
}
</style>
