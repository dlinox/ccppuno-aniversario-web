<template>
  <footer class="app-footer">
    <div class="logo-footer">
      <img src="/logo-cu.png" alt="" width="80px">
    </div>
    <div class="cr-footer">
      <p>© 2023 Colegio de Contadores Públicos de Puno.</p>
    </div>
  </footer>
</template>
<script setup>
</script>
<style lang="scss">
.app-footer{
  background-color: $secondary-color;

  .logo-footer{
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 1rem ;
    border-bottom: 1px dashed #eee;
  }
  .cr-footer{
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 1rem ;
    color: #AAA;
  }
}
</style>