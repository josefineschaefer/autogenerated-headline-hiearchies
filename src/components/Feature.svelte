<script>
	import { storyblokEditable } from '@storyblok/svelte';
	import { getHeadlineTag } from '../utils/getHeadlineTag';

	export let blok;
	export let index = null;

	const tag = getHeadlineTag(index);
</script>

<div use:storyblokEditable={blok} class="w-full p-12 bg-gradient-to-r from-[#EED3F5] to-[#dbd4f2] rounded-[5px] text-center">
	<svelte:element this={tag} class="text-2xl text-[#772D8B]">{blok.name}</svelte:element>
</div>
