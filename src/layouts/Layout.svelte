<script>
	export let templateHtml;
</script>

<!-- Global Head -->
<svelte:head>
	<link rel="stylesheet" type="text/css" href="/style.css">
</svelte:head>

<main>
	{@html templateHtml}
</main>
