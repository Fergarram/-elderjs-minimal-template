<script>
	import BlogTeaser from '../../components/BlogTeaser.svelte';
	export let data, helpers;
</script>

<svelte:head>
	<title>Elder.js Template: Home</title>
	<meta name="description" content="Elder.js Starter Template: It's A Tutorial Too!" />
	<link href="/" rel="canonical" />
</svelte:head>

<div>
	<h1>Blank Elder.js Template</h1>
	<p>This template asumes you have basic knowledge of how to use Elder.js. If you are wanting to learn more about all the bits and pieces then go ahead and use the official Elder.js template. I created this template for myself to be able to quick-start new projects, it's basically a slim fork of the original. I usually want to be ready to add TailwindCSS, SCSS, or PostCSS. So I might add this as an option or something.</p>
	<p>Here's a list of the main differences between this and the official template:</p>
	<ul>
		<li>
			I use tabs instead of spaces for all files.
		</li>
		<li>
			I removed prettier and eslint.
		</li>
		<li>
			I removed most examples only leaving placeholders for common things.
		</li>
	</ul>
</div>

<div>
	<h2>Blog listing example:</h2>
	<div>
		{#each data.markdown.blog as post}
			<BlogTeaser {post} {helpers} />
		{/each}
	</div>
</div>