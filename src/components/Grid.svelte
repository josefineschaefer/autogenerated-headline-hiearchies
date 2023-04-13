<script>
	import { storyblokEditable, StoryblokComponent } from '@storyblok/svelte';
	import { getHeadlineTag } from '../utils/getHeadlineTag';

	export let blok;
	export let index;
	const tag = getHeadlineTag(index);
</script>

<div use:storyblokEditable={blok}>
	<svelte:element this={tag} class="text-6xl text-center mb-8 mt-8 text-[#50b0ae] font-bold"
		>{blok.headline}</svelte:element
	>
	<div
		use:storyblokEditable={blok}
		class="container mx-auto grid md:grid-cols-3 gap-16 place-items-center"
	>
		{#each blok.columns as blok}
			<div class="flex-auto px-6">
				<StoryblokComponent {blok} />
			</div>
		{/each}
	</div>
</div>
