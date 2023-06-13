<template>
  <section class="section-container">
    <div class="header">
      <h1>Conception d’Achilleus</h1>
      <p>
        La conception d'un bot de trading a été motivée par plusieurs facteurs.
        Malgré une solide connaissance des stratégies de trading rentables
        telles que le price action et le wave trading, le biais émotionnel a
        posé problème : il était difficile de respecter un plan de trading en
        raison de l'avidité, de l'excès de confiance ou des pertes successives.
        De plus, il était compliqué de lâcher prise lorsqu'un trade était en
        cours. Un bot de trading fonctionnant 24h/24 sans émotion offre donc des
        avantages considérables.
      </p>
    </div>
    <div class="image-conception">
      <figure class="figure">
        <img
          src="../assets/conception-achilleus.jpg"
          alt="image illustrant la conception du bot Achilleus"
          class="conception-achilleus"
        />
      </figure>
    </div>
    <div class="details">
      <p>
        <img src="../assets/col1.png" class="image-column">
        La première étape a consisté à
        <b
          >concevoir une stratégie de trading algorithmique pouvant être
          traduite en langage Python</b
        >, puis à l'optimiser grâce au code en trouvant les meilleurs paramètres
        pour obtenir les meilleurs résultats. La stratégie utilisée par le bot a
        été testée sur 50 000 bougies (de mi-2017 à aujourd'hui), et le code a
        permis d'évaluer plus de 100 000 combinaisons de paramètres.
      </p>
      <p>
        <img src="../assets/col2.png" class="image-column">
        Un dernier filtre a été ajouté au bot,
        <b
          >un algorithme de machine learning (réseaux de neurones) qui détermine
          la probabilité de réaliser un take profit (TP) et un stop loss (SL)</b
        >
        en fonction des données du cours BTC/USDT. Ainsi, le bot ne passe un
        trade que lorsqu'un certain seuil de probabilité jugé favorable est
        atteint.
      </p>
      <div class="column">
        <img src="../assets/col3.png" class="image-column">
      Trois filtres optimisés sont appliqués avant l'entrée en position avec
      sur chacun d’eux
      <b>des conditions strictes :</b>
      <ul>
        <li>• L'entrée basée sur les bougies H4</li>
        <li>• La confirmation sur les bougies H1</li>
        <li>• La probabilité donnée par l'algorithme de machine learning</li>
      </ul>
    </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "ConceptionAchilleus",
};
</script>

<style scoped>
.section-container {
  padding: 1rem 6rem 1rem 6rem;
}
h1 {
  font-size: 2rem;
  font-weight: 700;
  line-height: 1;
  padding-bottom: 1rem;
}
.header {
  padding-bottom: 2rem;
}

.details {
  display: flex;
  padding-top: 2rem;
}
.details > * {
  margin: 0 2rem;
  flex: 1;
}

.column {
    gap: 1rem;
}

.image-column {
    width: 4rem;
    padding-bottom: 1rem;
    margin-top: -4rem;
}

ul {
    text-indent: 0.5rem;
    padding-top: 0.8rem;
}
</style>
