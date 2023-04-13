<script>
	import { storyblokEditable } from '@storyblok/svelte';
	import { getHeadlineTag } from '../utils/getHeadlineTag';

	export let blok;
	export let index = null;

	const tag = getHeadlineTag(index);
</script>

<div use:storyblokEditable={blok} class="w-full p-12 bg-[#f7f6fd] rounded-[5px] text-center">
	<svelte:element this={tag} class="text-2xl text-[#1d243d] font-bold">{blok.name}</svelte:element>
</div>
