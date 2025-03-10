<script>
	import '../app.css';
	let menuOpen = false;

</script>
<nav>
	<!-- svg button -->
	<a href="/" class="home-btn" aria-label="Home">
		<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="30" height="30" fill="white">
			<path d="M12 3l10 9h-3v9h-6v-6h-2v6H5v-9H2l10-9z"/>
		</svg>
	</a>

	<!-- svg button -->
	<button class="expand-btn" on:click={() => menuOpen = !menuOpen} aria-label="Expand Menu">
		<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" width="30" height="30" fill="white"
				 class:rotated={menuOpen}>
			<path d="M10 17l5-5-5-5v10z"/>
		</svg>
	</button>

	<!-- menu -->
	<div class="menu" class:open={menuOpen}>
		<a href="/arm" on:click={() => menuOpen = false}>Arm</a>
		<a href="/essay" on:click={() => menuOpen = false}>Essay</a>
		<a href="/source-code" on:click={() => menuOpen = false}>Source Code</a>
	</div>
</nav>

<main style="padding-top: 60px;">
	<slot />
</main>

<style>
    /* navbar */
    nav {
        width: 100vw;
        height: 60px;
        background: #222;
        display: flex;
        align-items: center;
        padding: 0 20px;
        position: fixed;
        top: 0;
        left: 0;
        box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.3);
    }

    /* home button */
    .home-btn {
        display: flex;
        align-items: center;
        justify-content: center;
        width: 50px;
        height: 50px;
        border-radius: 50%;
        background: #444;
        transition: background 0.3s;
        margin-right: 10px; /* 10 px between home button and arrow button */
    }

    .home-btn:hover {
        background: #2ecc71;
    }

    /* expand button */
    .expand-btn {
        display: flex;
        align-items: center;
        justify-content: center;
        width: 50px;
        height: 50px;
        border-radius: 50%;
        background: #444;
        cursor: pointer;
        border: none;
        transition: background 0.3s;
    }

    .expand-btn:hover {
        background: #555;
    }

    /* rotate the arrow */
    .rotated {
        transform: rotate(90deg);
        transition: transform 0.3s;
    }

    /* menu */
    .menu {
        display: flex;
        gap: 10px;
        background: #333;
        border-radius: 30px;
        padding: 10px 15px;
        position: absolute;
        left: 120px;
        top: 10px;
        opacity: 0;
        transform: scaleX(0);
        transform-origin: left;
        transition: opacity 0.3s, transform 0.3s;
        pointer-events: none;
    }

    /* when menu is open */
    .menu.open {
        opacity: 1;
        transform: scaleX(1);
        pointer-events: auto;
    }

    /* menu buttons */
    .menu a {
        display: block;
        padding: 10px 20px;
        color: white;
        text-decoration: none;
        border-radius: 20px;
        background: #444;
        transition: background 0.3s;
        text-align: center;
    }

    .menu a:hover {
        background: #2ecc71;
    }
</style>
