<div class="container">
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
  <div class="icon"></div>
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
  .container {
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
  }

  .allgemeines {
    grid-area: allgemeines;
  }

  .erholungsrate {
    grid-area: erholungsrate;
  }

  .icon {
    grid-area: icon;
    background-image: url(./img/Psycho-pass.logo.svg);
    background-size: contain;
    background-repeat: no-repeat;
    background-position: center;
  }

  .aspekte {
    grid-area: aspekte;
  }

  .methoden {
    grid-area: methoden;
  }

  .stunts {
    grid-area: stunts;
  }

  .stress {
    grid-area: stress;
  }

  .konsequenzen {
    grid-area: konsequenzen;
  }

  .column {
    display: flex;
    flex-direction: column;
    gap: 0.2rem;
  }

  textarea {
    resize: none;
  }

  .right {
    display: grid;
    gap: 0.2rem;
    grid-template-columns: auto 1fr;
  }

  .bottom {
    display: grid;
    gap: 0.2rem;
    grid-template-rows: auto 1fr;
  }
</style>
