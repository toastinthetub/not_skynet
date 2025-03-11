<h1>my senior project portfolio website :)</h1>
<h3>vite + react + rust backend</h3>

<p>USING GITHUB README AS A FILE TRANSFER FROM WORK COMPUTER:</p>
<code>
<script>
  let showOverlay = false;
</script>

<style>
  body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
  }

  button {
    position: absolute;
    top: 20px;
    right: 20px;
    padding: 10px 20px;
    font-size: 16px;
    cursor: pointer;
    background-color: #4CAF50;
    color: white;
    border: none;
    border-radius: 5px;
  }

  #overlay {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.7);
    opacity: {showOverlay ? 1 : 0};
    visibility: {showOverlay ? 'visible' : 'hidden'};
    transition: opacity 0.5s ease, visibility 0s 0.5s;
  }

  #options {
    position: fixed;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    display: flex;
    flex-direction: column;
    gap: 20px;
    opacity: {showOverlay ? 1 : 0};
    visibility: {showOverlay ? 'visible' : 'hidden'};
    transition: opacity 0.5s ease, visibility 0.5s ease;
  }

  .option {
    padding: 10px 20px;
    background-color: #fff;
    color: #333;
    border-radius: 5px;
    cursor: pointer;
    opacity: 0;
    transition: opacity 0.5s ease;
  }

  .option:nth-child(1) {
    transition-delay: 0.5s;
  }

  .option:nth-child(2) {
    transition-delay: 1s;
  }

  .option:nth-child(3) {
    transition-delay: 1.5s;
  }
</style>

<button on:click={() => showOverlay = !showOverlay}>
  Open Options
</button>

<div id="overlay"></div>

<div id="options">
  <div class="option">Option 1</div>
  <div class="option">Option 2</div>
  <div class="option">Option 3</div>
</div>
</code>
