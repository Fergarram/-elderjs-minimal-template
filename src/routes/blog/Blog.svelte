<script>
	export let data, request;
	const { html, frontmatter } = data;
</script>

<svelte:head>
	<title>{frontmatter.title}</title>
	<meta name="description" content={frontmatter.excerpt} />
	<link href={request.permalink} rel="canonical" />
</svelte:head>

<div class="title">
	<h1>{frontmatter.title}</h1>
	{#if frontmatter.author}<small>By {frontmatter.author}</small>{/if}
</div>

{#if html}
	{@html html}
{:else}
	<h1>Oops!! Markdown not found!</h1>
{/if}
