<script lang="ts">
	export let href = "#";
	export let variant: "primary" | "white" = "primary";
	export let size: "sm" | "md" = "md";
</script>

<a 
	{href} 
	class="
		inline-flex items-center justify-center gap-2 rounded-full font-medium transition-transform active:scale-95
		{variant === 'primary' ? 'bg-[#007AFF] text-white hover:bg-[#0062cc]' : 'bg-white text-black hover:bg-gray-50'}
		{size === 'sm' ? 'px-4 py-1.5 text-sm' : 'px-6 py-3 text-base'}
	"
>
	<slot />
</a>
