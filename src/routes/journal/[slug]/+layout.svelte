<script>
	export let data;
</script>

<div>
	<main>
		<slot />
	</main>
</div>
<aside>
	<h2>More Posts</h2>
	<ul>
		{#each data.summaries as { slug, title }}
			<li>
				<a href="/journal/{slug}">{title}</a>
			</li>
		{/each}
	</ul>
</aside>
