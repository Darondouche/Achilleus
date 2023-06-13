<template>
  <section class="section-container">
	<div class="image-container">
      <figure class="figure">
        <figcaption class="title">
          <span class="highlighted-text">Boost</span>
        </figcaption>
        <img
          src="../assets/achilleus_bot.jpg"
          alt="image illustrant le bot Boost"
          class="boost-image"
        />
      </figure>
	</div>
      <div class="text-container">
        <ul class="custom-list">
          <li>Name: Boost</li>
          <li>Création: 2042</li>
          <li>IQ: 399</li>
          <li>Favorite asset: Bitcoin</li>
          <li>Qualities: patient and sharp</li>
          <li>Yield: 400% in year 2022</li>
        </ul>
        <p class="description">
          Optimisez vos trades BTC/USDT avec Boost, le bot de trading
          futures 24/7.
          <br class="md-br" />Stratégie automatisée, gestion des risques,
          flexibilité du marché.
        </p>
        <div class="button-container">
          <a rel="noopener noreferrer" href="#" class="learn-more-button"
            >En savoir +</a
          >
          <a rel="noopener noreferrer" href="#" class="demo-button">Démo</a>
        </div>
      </div>
  </section>
</template>

<script>
export default {
  name: "BoostPresa",
};
</script>

<style scoped>
.section-container {
  background-color: #1f2937;
  display: flex;
  flex-direction: row;
  justify-content: center;
  color: #d1d5db;
  padding: 2rem;
}

.image-container {
  display: flex;
  flex-direction: column;
  width:100%;
}

.figure {
  margin:auto;
  width:80%;
}

.title {
  font-size: 2rem;;
  font-weight: 700;
  line-height: 1;
  padding: 1rem;
  text-align:center;
}

.highlighted-text {
  color: #10b981;
}

.boost-image {
  border-radius: 1rem;
  width: 100%;
}

.text-container {
  display: flex;
  flex-direction: column;
  margin:auto;
  padding-top:3rem;
}

.custom-list {
	font-family: 'Roboto Mono', monospace;
  color: #10b981;
}

.description {
  margin-top: 24px;
  margin-bottom: 32px;
  font-size: 16px;
}

.button-container {
  display: flex;
  flex-direction: row;
  gap: 4rem;
  justify-content: center;
  align-items: center;
}

.learn-more-button {
  padding: 12px 32px;
  font-size: 16px;
  font-weight: 600;
  border-radius: 6px;
  background-color: #10b981;
  color: #1f2937;
  text-decoration: none;
}

.demo-button {
  padding: 12px 32px;
  font-size: 16px;
  font-weight: 600;
  border-radius: 6px;
  border: 1px solid #d1d5db;
  color: #d1d5db;
  text-decoration: none;
}
</style>
