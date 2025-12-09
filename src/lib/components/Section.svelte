<script lang="ts">
	export let flip = false;
	export let contentBg = "";
	export let mediaBg = "";
    export let bgClass = "bg-white";
    export let fullHeight = false;
</script>

<section class="grid grid-cols-1 md:grid-cols-2 {fullHeight ? 'min-h-screen' : 'min-h-[600px]'} {bgClass}">
	<div class="flex flex-col justify-center p-8 md:p-16 lg:p-24 {contentBg} {flip ? 'md:order-2' : ''}">
		<slot name="content" />
	</div>
	<div class="flex items-center justify-center p-8 md:p-16 overflow-hidden relative {mediaBg} {flip ? 'md:order-1' : ''}">
		<slot name="media" />
	</div>
</section>
