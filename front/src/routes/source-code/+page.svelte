
<div class="page-container">
	<h1>PROJECT SOURCES...IF YOU WANT TO KNOW MORE ABOUT THE CODE.</h1>
	<p>I actually don't know any web development stuff at all...I had to scramble to learn how to make this website!</p>
	<div class="wrapper">
	<div class="grid-container">
		<a href="https://github.com/toastinthetub/">
			<img src="/src/assets/screenshot_one.png" alt="Screenshot One" />
		</a>
		<a href="https://github.com/toastinthetub/">
			<img src="/src/assets/screenshot_two.png" alt="Screenshot Two" />
		</a>
		<a href="https://github.com/toastinthetub/">
			<img src="/src/assets/screenshot_three.png" alt="Screenshot Three" />
		</a>
		<a href="https://github.com/toastinthetub/">
			<img src="/src/assets/screenshot_four.png" alt="Screenshot Four" />
		</a>
	</div>
	</div>
	<p><br>if you feel like checking any of those repos out, leave a star B)</p>>
</div>

<style>
    .wrapper {
        display: grid;
        place-items: center;
        height: 70vh;
    }
    .grid-container {
        display: grid;
        grid-template-columns: repeat(2, 1fr); /* 2 columns */
        grid-template-rows: repeat(2, 1fr); /* 2 rows */
        gap: 10px;
        width: 100vh;

    }

    a {
        display: block; /* Makes the entire image clickable */
    }

    img {
        width: 100%;
        height: 100%;
        object-fit: cover; /* Ensures images fill the squares */
        border-radius: 8px; /* Optional rounded corners */
        transition: transform 0.2s ease-in-out;
    }

    img:hover {
        transform: scale(1.05); /* Slight zoom on hover */
    }
</style>
