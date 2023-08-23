<template>
  <section class="event-description-container">
    <div class="container">
      <div class="event-description">
        <h2>Aniversario XX</h2>
        <p>
          Únete a nosotros en este grandioso aniversario del Colegio de
          Contadores de Puno. Una noche llena de sorpresas, reencuentros y, por
          supuesto, ¡música en vivo! No querrás perderte a nuestras estrellas de
          la noche:
        </p>
        <ul class="bands-list">
          <li>Grupo Alma Bella</li>
          <li>Agrupación La Pachanga</li>
        </ul>
      </div>
      <div class="event-image">
        <img src="/static/images/second-img.jpg" alt="Imagen del evento" />
      </div>
    </div>
  </section>
</template>

<style lang="scss">
.event-description-container {
  display: flex;
  align-items: center;
  height: 80vh;
  overflow: hidden;
  // background-image: url("/static/images/bg-second.jpg");

  background: linear-gradient(
      45deg,
      rgba($secondary-color, 0.5),
      rgba($secondary-color, 0.5)
    ),
    url("/static/images/bg-second.jpg") center center / cover no-repeat;

  // background: radial-gradient(
  //     circle at top left,
  //     rgba(#000040, 0.3) 20%,
  //     transparent
  //   ),
  //   radial-gradient(circle at bottom right, rgba(#000040, 0.3) 20%, transparent),
  //   linear-gradient(45deg, rgba(#000045, 0.3) 50%, #000040 50%)
  //     url("/static/images/bg-second.jpg");
  // background-blend-mode: overlay, overlay, overlay;

  .container {
    display: flex;
    align-items: center;
    height: 100%;
    .event-description {
      flex: 1;
      padding: 5vh 5vw; // padding relativo al viewport
      overflow-y: auto; // en caso de que el contenido exceda el alto

      h2 {
        font-size: 3.5em;
        color: white;
        margin-bottom: 20px;
        text-shadow: 4px 4px 4px $secondary-color;
      }

      p {
        font-size: 1.2em;
        margin-bottom: 20px;
        color: white;
      }

      .bands-list {
        list-style: none;

        li {
          font-size: 1.5em;
          font-weight: bold;
          color: white;
          margin-bottom: 0.8rem;

          &:before {
            content: "🎵";
            margin-right: 10px;
          }
        }
      }
    }

    .event-image {
      flex: 1;
      display: flex;
      align-items: center;
      justify-content: center;

      img {
        width: 100%;
        height: 100%;
        object-fit: cover;
      }
    }

    // Responsivo: Si la pantalla es pequeña, muestra la descripción arriba y la imagen abajo
    @media (max-width: 768px) {
      flex-direction: column;

      .event-description,
      .event-image {
        flex: none;
        width: 100%;
      }
    }
  }
}
</style>
