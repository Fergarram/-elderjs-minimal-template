<script>
	export let post;
	export let helpers;
</script>

<div class="entry">
	<a href={helpers.permalinks.blog({ slug: post.slug })}>{post.frontmatter.title}</a>
	<p>{post.frontmatter.excerpt}</p>
</div>
