Drücke `Strg`+ `P` zum drucken.

<div class="character-sheet">
  <div
    class="allgemeines column"
    style="display: grid; gap: 0.2rem; grid-template-rows: auto auto 1fr"
  >
    <h2>Allgemeines</h2>
    <label class="right">Name<input type="text" /></label>
    <label class="bottom">Beschreibung<textarea></textarea></label>
  </div>
  <label class="erholungsrate bottom"
    >Erholungsrate
    <textarea></textarea>
  </label>
  <div class="icon">
    <img src="./img/Psycho-pass.logo.svg" />
  </div>
  <div
    class="aspekte"
    style="display: grid; grid-template-rows: auto repeat(5, 1fr); gap: 0.2rem"
  >
    <h2>Aspekte</h2>
    <label class="right">Konzept<input type="text" /></label>
    <label class="right">Dilemma<input type="text" /></label>
    <input type="text" />
    <input type="text" />
    <input type="text" />
  </div>
  <div
    class="methoden column"
    style="display: grid; grid-template-rows: auto repeat(6, 1fr); gap: 0.2rem"
  >
    <h2>Methoden</h2>
    <label class="right">Flink<input type="text" /></label>
    <label class="right">Kraftvoll<input type="text" /></label>
    <label class="right">Scharfsinnig<input type="text" /></label>
    <label class="right">Sorgfältig<input type="text" /></label>
    <label class="right">Tollkühn<input type="text" /></label>
    <label class="right">Tückisch<input type="text" /></label>
  </div>
  <div class="stunts bottom">
    <h2>Stunts</h2>
    <textarea></textarea>
  </div>
  <div class="stress bottom">
    <h2>Stress</h2>
    <div
      style="display: grid; grid-template-columns: repeat(3, 1fr); gap: 0.2rem"
    >
      <label class="bottom" style="height: 100%">1<input /></label>
      <label class="bottom" style="height: 100%">2<input /></label>
      <label class="bottom" style="height: 100%">3<input /></label>
    </div>
  </div>
  <div
    class="konsequenzen"
    style="display: grid; grid-template-rows: auto repeat(3, 1fr); gap: 0.2rem"
  >
    <h2>Konsequenzen</h2>
    <label class="right">2<input placeholder="Leicht" /></label>
    <label class="right">4<input placeholder="Mittel" /></label>
    <label class="right">6<input placeholder="Schwer" /></label>
  </div>
</div>

<style>
  @media print {
    .character-sheet {
      max-height: 100vh !important;
    }

    .markdown-body > p,
    .markdown-body > h1,
    .markdown-body > .footer {
      display: none !important;
      visibility: collapse !important;
    }
  }

  .character-sheet {
    display: grid;
    grid-template-columns: 1fr 0.5fr 1fr;
    grid-template-rows: repeat(7, 1fr);
    gap: 1rem;
    grid-auto-flow: row;
    grid-template-areas:
      "allgemeines allgemeines icon"
      "allgemeines allgemeines erholungsrate"
      "aspekte aspekte methoden"
      "aspekte aspekte methoden"
      "stunts stunts stunts"
      "stunts stunts stunts"
      "stress konsequenzen konsequenzen";
    max-width: 100%;
  }

  .character-sheet > .allgemeines {
    grid-area: allgemeines;
  }

  .character-sheet > .erholungsrate {
    grid-area: erholungsrate;
  }

  .character-sheet > .icon {
    grid-area: icon;
  }

  .character-sheet > .aspekte {
    grid-area: aspekte;
  }

  .character-sheet > .methoden {
    grid-area: methoden;
  }

  .character-sheet > .stunts {
    grid-area: stunts;
  }

  .character-sheet > .stress {
    grid-area: stress;
  }

  .character-sheet > .konsequenzen {
    grid-area: konsequenzen;
  }

  .character-sheet .column {
    display: flex;
    flex-direction: column;
    gap: 0.2rem;
  }

  .character-sheet textarea {
    resize: none;
  }

  .character-sheet .right {
    display: grid;
    gap: 0.2rem;
    grid-template-columns: auto 1fr;
  }

  .character-sheet .bottom {
    display: grid;
    gap: 0.2rem;
    grid-template-rows: auto 1fr;
  }
</style>
