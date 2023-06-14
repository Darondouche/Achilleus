<template>
  <section class="section-container">
    <div class="header">
      <h1>Limites du bot de trading et avertissements</h1>
      <p>
        Un bot de trading algorithmique est optimisé en fonction des données
        passées,
        <b
          >ce qui ne garantit pas nécessairement des performances identiques à
          l'avenir.</b
        >
        Cependant, afin de limiter le "biais de sur-apprentissage", le backtest
        a été effectué en utilisant des tranches de données d'entraînement et de
        test. De plus, la stratégie semble rentable sur des données totalement
        nouvelles, car elle a été testée sur le cours ETH/USDT et les
        performances sont similaires.
      </p>
      <br />
      <p>
        Ce que nous proposons sur le canal Telegram, ce sont les
        <b
          >signaux des trades effectués par le bot en temps réel, incluant tous
          les paramètres du trade</b
        >
        (point d'entrée, stop loss et levier). Contrairement à de nombreuses
        "arnaques", les signaux sont détaillés et correspondent à des trades
        réellement effectués par le bot. Il est néanmoins essentiel d'être en
        mesure de
        <b
          >passer manuellement un ordre sur un compte de trading à terme et
          d'avoir une expérience minimale en trading</b
        >
        pour tirer pleinement profit des signaux.
      </p>
      <br />
      <p>
        Pour ceux qui préfèrent l'investissement en spot, nous vous invitons à
        découvrir notre deuxième bot : le bot d'investissement Spot.
      </p>
    </div>
    <div class="image-limits">
      <figure class="figure">
        <img
          src="../assets/limitsAchilleus.jpg"
          alt="image de signal d'avertissement"
          class="limits-achilleus"
        />
      </figure>
      <a rel="noopener noreferrer" href="#">
        <div class="button-container">
          <img src="../assets/telegram.png" alt="logo telegram" class="logo" />
          <p>Rejoindre Télégram</p>
        </div>
      </a>
    </div>
  </section>
</template>

<script>
export default {
  name: "LimitsAchilleus",
};
</script>

<style scoped>
.section-container {
  padding: 4rem 3rem 2rem 3rem;
  display: flex;
  background-color: black;
  width: 90%;
  border-radius: 2rem;
  margin: auto;
  margin-top: 3rem;
}

h1 {
  font-size: 2rem;
  font-weight: 700;
  line-height: 1;
  padding-bottom: 2rem;
}
.header {
  padding-bottom: 2rem;
  gap: 1rem;
}

.image-limits {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-around;
}
.button-container {
  height: 3rem;
  width: 16rem;
  display: flex;
  flex-direction: row;
  gap: 1rem;
  justify-content: center;
  align-items: center;
  font-weight: 600;
  border-radius: 0.4rem;
  background-color: #9833d1;
  color: #ffffff;
  text-decoration: none;
}

.logo {
  width: 1.9rem;
}

</style>
