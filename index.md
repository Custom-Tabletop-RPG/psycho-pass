<img src="https://frank-mayer.github.io/psycho-pass-pnp/img/Psycho-pass.logo.svg" style="width:min(85%,600px);margin:4rem auto;display:block;height:auto;" />

## Inhaltsverzeichnis

- [Story](/story.md)
- [Karte](/karte.md)
- [Regelwerk](/regelwerk.md)
- [Charakterbogen](/charakterbogen.md)

<div class="cover">
    <img class="kogami" src="https://frank-mayer.github.io/psycho-pass-pnp/img/kogami.webp"/>
    <img class="makishima" src="https://frank-mayer.github.io/psycho-pass-pnp/img/makishima.webp"  />
</div>

<style>
@media print {
  .cover {
    display: none !important;
  }
}

h1 {
  display: none !important;
}

.cover {
  width: min(800px, 100%);
  margin: 0 auto;
  display: grid; 
  grid-template-columns: repeat(3, 1fr); 
  grid-template-rows: repeat(3, 1fr); 
  gap: 0; 
}

.cover img {
  background: none !important;
}

@media only screen and (max-width: 600px) {
  .kogami { grid-area: 1 / 1 / 4 / 3; }
  .makishima { grid-area: 2 / 2 / 4 / 4; }
}

@media only screen and (min-width: 600px) {
  .kogami { grid-area: 1 / 1 / 3 / 3; }
  .makishima { grid-area: 2 / 2 / 4 / 4; }
}
</style>
