<script>
	import Title from "$lib/Title.svelte";

export let data
</script>
<Title name="blog" />

<section>
	<div class="outer">
		<div class="inner auto-fit">

			{#each data.posts.posts as post}
				<div class="flow">
				<img src="{post.featured_image}" alt="{post.title}">
				<h2><a href="/blog/{post.slug}">{@html post.title}</a></h2>
				<p>{@html post.excerpt}</p>
			</div>
			{/each}
			
		</div>
	</div>
</section>