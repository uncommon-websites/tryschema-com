<script lang="ts">
	export let bgClass = "bg-white";
	export let dark = false;
</script>

<div class="relative mx-auto border-gray-800 dark:border-gray-800 bg-gray-900 border-[12px] rounded-[3.5rem] h-[640px] w-[310px] shadow-2xl flex flex-col overflow-hidden {bgClass} ring-1 ring-gray-900/5">
    <!-- Dynamic Island -->
    <div class="absolute top-3 left-1/2 transform -translate-x-1/2 h-[28px] w-[100px] bg-black rounded-full z-20 flex items-center justify-between px-3">
        <div class="w-2 h-2 rounded-full bg-[#1a1a1a]"></div>
        <div class="w-2 h-2 rounded-full bg-[#1a1a1a]"></div>
    </div>
    
    <!-- Status Bar Time -->
    <div class="absolute top-4 left-9 text-[13px] font-semibold z-20 tracking-wide {dark ? 'text-white' : 'text-black'}">9:41</div>
    
    <!-- Status Bar Icons -->
    <div class="absolute top-4 right-9 flex gap-1.5 z-20 items-center">
        <svg class="w-4 h-3 {dark ? 'text-white' : 'text-black'}" viewBox="0 0 18 12" fill="currentColor">
             <path d="M14 1h-3v10h3V1zm-4.5 2h-3v8h3V3zm-4.5 3h-3v5h3V6z"/>
        </svg>
        <div class="w-5 h-3 rounded-[3px] border-[1.5px] {dark ? 'border-white' : 'border-black'} relative opacity-40">
            <div class="absolute top-[1.5px] left-[1.5px] bottom-[1.5px] right-[1.5px] {dark ? 'bg-white' : 'bg-black'}"></div>
        </div>
    </div>

    <!-- Screen Content -->
    <div class="flex-1 w-full h-full overflow-hidden relative z-10">
        <slot />
    </div>
</div>
