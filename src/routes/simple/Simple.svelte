<script>
	export let data, request;
</script>

<svelte:head>
	<title>Simple</title>
	<meta name="description" content="A Simple Route" />
	<link href={request.permalink} rel="canonical" />
</svelte:head>

<h1>Simple</h1>

{@html data.content}
