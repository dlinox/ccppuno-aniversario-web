<template>
  <section class="pricing-section">
    <div class="container">
      <h2>Precios</h2>
      <div class="price-card">
        <h4>Hábiles</h4>
        <p class="price">S/. 20.00</p>
      </div>
      <div class="price-card">
        <h4>Inhábiles y Público en General</h4>
        <p class="price">S/. 50.00</p>
      </div>
      <div class="btn-content">
        <button class="btn btn-outline-primary">
          conseguir entradas
        </button>
      </div>
    </div>
  </section>
</template>
<style lang="scss">
.pricing-section {
  padding: 50px 0;
  background-color: black;
  color: white;

  background: linear-gradient(
      45deg,
      rgba(black, 0.96),
      rgba(black, 0.96)
    ),
    url("/static/images/bd-f.jpg") center center / cover no-repeat;


  .container {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    h2 {
      width: 100%;
      font-size: 2.5em;
      color: white;
      margin-bottom: 2.5rem;
    }
    .price-card {
      width: 45%;
      background-color: rgba(200, 200, 200, 0.1);
      padding: 30px;
      border-radius: 8px;
      text-align: center;
      transition: transform 0.3s ease;
      margin-bottom: 20px; // Espacio entre tarjetas si se apilan verticalmente en pantallas estrechas

      &:hover {
        transform: translateY(-10px);
      }

      h4 {
        margin-bottom: 20px;
        font-size: 1.5rem;
      }

      .price {
        font-size: 2rem;
        font-weight: bold;
        color: $highlight-color;
      }
    }

    .btn-content{
      padding: 2rem;
      width: 100%;
      display: flex;
      align-items: center;
      justify-content: center;
    }
  }
}
</style>
