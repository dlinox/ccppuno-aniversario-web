<template>
  <section class="first-section">
    <div class="container banner-contnet">
      <h1 class="">
        ¡Celebra con Nosotros <br />
        <span>el Gran Aniversario del Colegio de Contadores de Puno!</span>
      </h1>

      <div class="date-container">
        <span class="day">11</span>
        <div class="month-year">
          <span class="month">SEPTIEMBRE</span>
          <span class="year">2023</span>
        </div>
      </div>
    </div>
  </section>
</template>
<script setup></script>
<style lang="scss">
.first-section {
  width: 100%;
  height: 100vh;
  background-image: url("/static/images/image-section-first.jpg");
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
  z-index: 1; // Asegura que el contenido del botón esté encima
  display: flex;
  align-items: center;

  &::after {
    content: "";
    position: absolute;
    width: 100%;
    height: 100%;
    top: 0;
    left: 0;
    background: linear-gradient(
      to bottom right,
      rgba($primary-color, 0.4),
      rgba(13, 56, 128, 0.6)
    );
    z-index: -1;
  }
  .container {
    &.banner-contnet {
      padding-top: 3rem;
      text-align: end;
      color: white;
      h1 {
        font-size: 4.5rem;
        text-shadow: 2px 2px 4px rgba($secondary-color, 0.4);
        span {
          text-shadow: 4px 4px 6px rgba($primary-color, 0.4);
        }
      }

      .date-container {
        backdrop-filter: blur(4px); // Desenfoque para el fondo
        -webkit-backdrop-filter: blur(
          4px
        ); // Para soporte en navegadores WebKit (Safari)

        display: inline-flex;
        background: rgba(255,255,255, 0.1);

        border-radius: 8px;
        padding: 10px 20px;
        box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2); // Sombra para el efecto "elevado"

        .day {
          font-size: 4em;
          font-weight: bold;
          margin-right: 1rem;
          color: $primary-color;
          border-right: 2px solid white;
         
          padding-right: 10px;
        }

        .month-year {
          display: flex;
          flex-direction: column;
          align-items: start;
          justify-content: center;

          .month {
            font-size: 1.5em;
            font-weight: bold;
            color: $primary-color;
          }

          .year {
            color: white;
          }
        }
      }
    }
  }
}
</style>
