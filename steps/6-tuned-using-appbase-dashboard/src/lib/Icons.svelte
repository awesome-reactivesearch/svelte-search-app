<script>
	export let suggestionType = 'index';
</script>

{#if suggestionType === 'popular'}
	<svg
		xmlns="http://www.w3.org/2000/svg"
		height="20"
		width="20"
		viewBox="0 0 24 24"
		style="fill: #707070"
	>
		<path d="M0 0h24v24H0z" fill="none" />
		<path d="M16 6l2.29 2.29-4.88 4.88-4-4L2 16.59 3.41 18l6-6 4 4 6.3-6.29L22 12V6z" />
	</svg>
{:else if suggestionType === 'recent'}
	<svg
		xmlns="http://www.w3.org/2000/svg"
		height="20"
		width="20"
		viewBox="0 0 24 24"
		style="fill: #707070"
	>
		<path d="M0 0h24v24H0z" fill="none" />
		<path
			d="M13 3c-4.97 0-9 4.03-9 9H1l3.89 3.89.07.14L9 12H6c0-3.87 3.13-7 7-7s7 3.13 7 7-3.13 7-7 7c-1.93 0-3.68-.79-4.94-2.06l-1.42 1.42C8.27 19.99 10.51 21 13 21c4.97 0 9-4.03 9-9s-4.03-9-9-9zm-1 5v5l4.28 2.54.72-1.21-3.5-2.08V8H12z"
		/>
	</svg>
{:else if suggestionType === 'promoted'}
	<svg
		xmlns="http://www.w3.org/2000/svg"
		width="20"
		height="20"
		viewBox="0 0 24 24"
		style="fill: #707070"
	>
		<path
			d="M12 .587l3.668 7.568 8.332 1.151-6.064 5.828 1.48 8.279-7.416-3.967-7.417 3.967 1.481-8.279-6.064-5.828 8.332-1.151z"
		/>
	</svg>
{:else}
	<svg class="search-icon" height="12" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 15 15">
		<title>Search</title>
		<path
			d="
        M6.02945,10.20327a4.17382,4.17382,0,1,1,4.17382-4.17382A4.15609,4.15609,
        0,0,1,6.02945,10.20327Zm9.69195,4.2199L10.8989,9.59979A5.88021,5.88021,
        0,0,0,12.058,6.02856,6.00467,6.00467,0,1,0,9.59979,10.8989l4.82338,
        4.82338a.89729.89729,0,0,0,1.29912,0,.89749.89749,0,0,0-.00087-1.29909Z
      "
		/>
	</svg>
{/if}

<style>
	.search-icon {
		transform: scale(1.35);
		position: relative;
		fill: rgb(112, 112, 112);
		left: 1px;
	}
</style>
