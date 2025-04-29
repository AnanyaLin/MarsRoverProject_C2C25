<script lang="ts">
	let { children } = $props();
</script>

<nav>
	<a href="/">home</a>
	<a href="/results">results</a>
</nav>

{@render children()}

<style>
	/* Styles the main content area */
	main {
		max-width: 800px; /* Limits the width of the main area */
		margin: 2rem auto; /* Centers the main area with vertical spacing */
		padding: 2rem; /* Adds space inside the main area */
		background: #fffbe7; /* Sets a light background color */
		border-radius: 12px; /* Rounds the corners */
		border: 2px solid #ebbbd6; /* Adds a light pink border */
	}

	/* Changes the color of all h1, h2, and h3 headings */
	:global(h1),
	:global(h2),
	:global(h3) {
		color: #e23089; /* Sets heading text color to a bright pink */
	}

	/* Styles all button elements */
	:global(button) {
		background: #e5acd3; /* Sets button background to light pink */
		color: #fff; /* Sets button text to white */
		border: none; /* Removes default border */
		border-radius: 6px; /* Rounds the button corners */
		padding: 0.5em 1em; /* Adds space inside the button */
		font-size: 1em; /* Sets button text size */
		cursor: pointer; /* Shows pointer cursor on hover */
	}

	/* Changes button background color when hovered */
	:global(button:hover) {
		background: #d85498; /* Changes background to red on hover */
	}
</style>

