<script lang="ts">
	import Metadata from '$lib/components/metadata.svelte';

	import type { PageProps } from './$types';

	let { data }: PageProps = $props();
</script>

<Metadata title={data.meta.title + ' | CyR1en'} description={data.meta.description} image={data.meta.poster} />

<header class="group border-cat-surface0 bg-cat-surface0 relative mb-5 aspect-[3/1] overflow-hidden border">
	<img src={data.meta.poster} alt={data.meta.title} class="size-full object-cover object-center" />
	<div class="absolute top-0 left-0 grid h-full w-full place-items-center bg-[#080808]/80 transition-opacity duration-500 group-hover:opacity-0">
		<h1 class="max-w-[80%] px-4 text-center text-2xl font-semibold uppercase lg:max-w-[60%] lg:text-4xl">
			{data.meta.title}
		</h1>
	</div>
	<div
		aria-hidden="true"
		class="absolute top-0 left-0 h-full w-full bg-repeat opacity-[2%] group-hover:opacity-0"
		style="background-image: url('https://framerusercontent.com/images/rR6HYXBrMmX4cRpXfXUOvpvpB0.png')"
	></div>
</header>

<article
	class="prose prose-hr:border-surface1 prose-pre:bg-cat-base/20 prose-code:before:opacity-0 prose-code:after:opacity-0 prose-code:text-cat-subtext1 prose-code:font-mono prose-pre:border prose-headings:text-cat-text prose-p:text-cat-subtext1 prose-strong:text-cat-text prose-li:text-cat-subtext1 prose-li:marker:text-cat-subtext0 prose-a:text-cat-mauve prose-blockquote:border-cat-overlay2 prose-p:indent-5 prose-td:text-cat-subtext1 prose-thead:border-cat-subtext1 prose-tr:border-ash-500 mx-auto max-w-3xl font-sans"
>
	<data.content />
</article>
