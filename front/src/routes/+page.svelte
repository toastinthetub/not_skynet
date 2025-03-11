<!-- >https://coolors.co/fffcf2-ccc5b9-403d39-252422-eb5e28 <-->

<div class="big-bang-text">
    PORTFOLIO.
</div>
<div class="flex justify-center">
    <div class="centered">(sam's senior project e-portfolio)</div>
</div>
<div class="divider-container">
    <div class="divider"></div>
</div>
<div class="grid-container-container">
<div class="grid-container">
    <a href="/arm">
    <div class="grid-item">
        <img src="/src/assets/misc-assets/robot-arm-screenshot-one.png" alt="a">
        <p class="centered-text">ARM</p>
    </div>
    </a>
    <a href="/essay">
    <div class="grid-item">
        <img src="/src/assets/misc-assets/essay-one.png" alt="b">
        <p class="centered-text">WRITEUP</p>
    </div>
    </a>
    <a href="/source-code">
    <div class="grid-item">
        <img src="/src/assets/misc-assets/screenshot_three.png" alt="c">
        <p class="centered-text">SOURCE CODE</p>
    </div>
    </a>
</div>
</div>
<div class="divider-container">
<div class="divider"></div>
</div>
<div class="divider-container">
    <a href="https://github.com/toastinthetub/not_skynet" class="special-link">
    <br>this website was fun to make! check out the src
    </a>
</div>

<style>
    .divider-container {
        display: flex;
        justify-content: center;
    }
    .divider {
        width: 75%;
        height: 2px;
        background-color: black;
        margin-top: 20px;
    }
    .centered {
        display: flex;
        justify-content: center;
        align-items: center;
        margin-top: 33vh;
        font-family: 'Courier New', Courier, monospace;
    }
    .grid-container-container {
        display: flex;
        justify-content: center;
    }
    /* Set up the grid */
    .grid-container {
        padding-top: 15px;
        justify-items: center; /* center grid items horizontally */
        align-items: flex-start;
        display: grid;
        grid-template-columns: repeat(3, 1fr); /* 1x3 grid */
        gap: 10px;

    }

    .grid-item {
        position: relative;
        border-radius: 15px; /* round corners */
        border: 1px solid #EB5E28;
        overflow: hidden;
        cursor: pointer;
        height: 25vh;
        width: 25vw;
    }

    .grid-item img {
        width: 100%;
        height: 100%;
        object-fit: cover;
        transition: filter 0.3s ease-in-out;
    }

    .centered-text {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        color: white;
        font-size: 20px;
        font-weight: normal; /* normal text weight initially */
        text-align: center;
        z-index: 1;
        transition: font-weight 0.3s ease-in-out; /* smooth */
    }

    /* image hover effects */
    .grid-item:hover img {
        filter: blur(5px); /* blur image */
    }

    .grid-item:hover .centered-text {
        font-weight: bold;
    }
</style>