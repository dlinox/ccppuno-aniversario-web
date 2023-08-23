<template>
  <section class="third-secction">
    <div
      class="band-item"
      style="
        background: linear-gradient(
            45deg,
            rgba(0, 0, 0, 0.5),
            rgba(0, 0, 0, 0.5)
          ),
          url('/static/images/alma-bella.jpg') center center / cover no-repeat;
      "
    >
      <div class="band-name">GRUPO ALMA BELLA</div>
    </div>
    <div
      class="band-item"

      style="
        background: linear-gradient(
            45deg,
            rgba(0, 0, 0, 0.5),
            rgba(0, 0, 0, 0.5)
          ),
          url('/static/images/la-pachanga.jpg') center center / cover no-repeat;
      "
    >
      <div class="band-name">AGRUPACION LA PACHANGA</div>
    </div>
  </section>
</template>
<style lang="scss">
.third-secction {
  background-color: black;
  display: grid;
  height: 50vh;
  grid-template-columns: 1fr 1fr; // Dos columnas iguales
  overflow: hidden;
  .band-item {
    height: 100%px; // o cualquier altura que prefieras
    position: relative;
    background-size: cover;
    background-position: center;
    cursor: pointer;
    transition: transform 0.3s ease;
    overflow: hidden;

    &:hover {
      transform: scale(1.05); // Aumento de tamaño al pasar el ratón por encima

      .band-name {
        opacity: 1; // Mostrar el nombre de la banda al pasar el ratón por encima
      }
    }

    .band-name {
      position: absolute;
      bottom: 10%;
      left: 50%;
      transform: translateX(-50%); // Centrar horizontalmente
      background-color: rgba(0, 0, 0, 0.7); // Fondo semitransparente
      padding: 5px 10px;
      border-radius: 5px;
      opacity: 0; // Inicialmente oculto
      transition: opacity 0.3s ease;
      color: white; // Color del texto
    }
  }
}
</style>
