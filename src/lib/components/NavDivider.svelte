<script lang="ts">
	export let active: "Meet Schema" | "Databases" | "Editing" | "Tools" = "Meet Schema";

	const items = ["Meet Schema", "Databases", "Editing", "Tools"];
</script>

<div class="py-24 px-6 md:px-12 max-w-7xl mx-auto">
	<div class="flex flex-col gap-2">
		{#each items as item}
			<div class="flex items-center gap-4 text-3xl md:text-5xl font-bold tracking-tight transition-colors duration-300 {active === item ? 'text-black' : 'text-gray-300'}">
				{#if active === item}
					<svg viewBox="0 0 24 24" fill="none" class="w-8 h-8 md:w-12 md:h-12 stroke-current stroke-[2.5]">
						<path d="M5 12H19M19 12L12 5M19 12L12 19" stroke-linecap="round" stroke-linejoin="round"/>
					</svg>
				{/if}
				<span class={active === item ? "" : "pl-12 md:pl-16"}>{item}</span>
			</div>
		{/each}
	</div>
</div>
