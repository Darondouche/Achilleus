<template>
  <section class="section-container">
    <div class="text-container">
      <div class="texts">
        <ul class="custom-list">
          <li>Name: 'Eμμa</li>
          <li>Origine: Cypherpunk's Haven</li>
          <li>Trading style: Spot investment</li>
          <li>Qualities: decisive and confident</li>
          <li>Flaw: hates shitcoins and scammers</li>
          <li>Favorite asset: Bitcoin</li>
        </ul>
        <p class="description">
          Surpassez le marché avec notre bot d'investissement en cryptomonnaies. Profitez de signauxd'achat et de vente judicieux pour optimisez vos profits.
          <br class="md-br" />Cliquez pour en savoir plus.
        </p>
      </div>
      <div class="button-container">
        <a rel="noopener noreferrer" href="#" class="learn-more-button"
          >En savoir +</a
        >
        <a rel="noopener noreferrer" href="#" class="demo-button">Démo</a>
      </div>
    </div>
    <div class="image-container">
      <figure class="figure">
        <figcaption class="title">
          <span class="highlighted-text">Bot Spot Invest</span>
        </figcaption>
        <img
          src="../assets/SpotInvest.jpg"
          alt="image illustrant le bot Spot Invest"
          class="emma-image"
        />
      </figure>
    </div>
  </section>
</template>

<script>
export default {
  name: "SpotInvestPresa",
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
  width: 100%;
}

.figure {
  margin: auto;
  width: 80%;
}

.title {
  font-size: 2rem;
  font-weight: 700;
  line-height: 1;
  padding: 1rem;
  text-align: center;
}

.highlighted-text {
  color: #10b981;
}

.emma-image {
  border-radius: 1rem;
  width: 100%;
}

.text-container {
  display: flex;
  flex-direction: column;
  margin: auto;
  padding-top: 3rem;
}

.texts {
  text-align: end;
}

.custom-list {
  font-family: "Roboto Mono", monospace;
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
