<script lang="ts">
	import NavDivider from "$lib/components/NavDivider.svelte";
	import Phone from "$lib/components/Phone.svelte";
	import Section from "$lib/components/Section.svelte";
	import Button from "$lib/components/Button.svelte";
	import Apple from "$lib/icons/Apple.svelte";
    import Search from "$lib/icons/Search.svelte";
</script>

<div class="w-full overflow-x-hidden bg-white">
	<!-- Header -->
	<header class="fixed top-0 left-0 right-0 z-50 flex items-center justify-between px-6 py-4 bg-white/80 backdrop-blur-md">
		<div class="w-8 h-8 bg-blue-500 rounded-lg flex items-center justify-center text-white font-bold text-lg">S</div>
		<Button size="sm" variant="primary">Get Schema</Button>
	</header>

	<!-- Hero Section -->
	<Section>
		<div slot="content" class="space-y-6">
			<h1 class="text-5xl md:text-6xl font-semibold tracking-tight text-gray-900">
				Databases for iOS.
			</h1>
			<p class="text-lg text-gray-500 max-w-md leading-relaxed">
				Schema is a powerful new database client for iOS. Built with the latest technologies, designed for clarity, and focused on handling the tasks when you aren't at a desk.
			</p>
			<div class="pt-4">
				<Button>Get Schema</Button>
			</div>
            <div class="pt-12 flex gap-1">
                <div class="w-2 h-2 rounded-full bg-black"></div>
                <div class="w-2 h-2 rounded-full bg-gray-300"></div>
                <div class="w-2 h-2 rounded-full bg-gray-300"></div>
                <div class="w-2 h-2 rounded-full bg-gray-300"></div>
            </div>
		</div>
		<div slot="media" class="relative">
			<Phone bgClass="bg-blue-500">
				<div class="flex flex-col h-full text-white p-6 pt-12">
					<div class="text-3xl font-bold mt-8 mb-4">SCHEMA</div>
                    
                    <!-- Search Bar Mockup -->
                    <div class="bg-blue-400/50 h-10 rounded-xl flex items-center px-3 mb-8">
                         <Search class="w-5 h-5 opacity-70" />
                         <span class="ml-2 opacity-70 text-sm">Search</span>
                    </div>

                    <div class="bg-white rounded-2xl flex-1 overflow-hidden text-black p-4">
                        <div class="text-lg font-bold mb-4">Production</div>
                        <div class="space-y-4">
                             <div class="flex items-center gap-3 p-2">
                                 <div class="w-8 h-8 rounded-full bg-blue-100 flex items-center justify-center text-blue-500">
                                     <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 7v10c0 2.21 3.582 4 8 4s8-1.79 8-4V7M4 7c0 2.21 3.582 4 8 4s8-1.79 8-4M4 7c0-2.21 3.582-4 8-4s8 1.79 8 4m0 5c0 2.21-3.582 4-8 4s-8-1.79-8-4"></path></svg>
                                 </div>
                                 <span class="font-medium text-lg">Peaberry</span>
                             </div>
                             <div class="flex items-center gap-3 p-2">
                                 <div class="w-8 h-8 rounded-full bg-blue-100 flex items-center justify-center text-blue-500">
                                     <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 7v10c0 2.21 3.582 4 8 4s8-1.79 8-4V7M4 7c0 2.21 3.582 4 8 4s8-1.79 8-4M4 7c0-2.21 3.582-4 8-4s8 1.79 8 4m0 5c0 2.21-3.582 4-8 4s-8-1.79-8-4"></path></svg>
                                 </div>
                                 <span class="font-medium text-lg">Starcee</span>
                             </div>
                             <div class="flex items-center gap-3 p-2">
                                 <div class="w-8 h-8 rounded-full bg-blue-100 flex items-center justify-center text-blue-500">
                                     <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 7v10c0 2.21 3.582 4 8 4s8-1.79 8-4V7M4 7c0 2.21 3.582 4 8 4s8-1.79 8-4M4 7c0-2.21 3.582-4 8-4s8 1.79 8 4m0 5c0 2.21-3.582 4-8 4s-8-1.79-8-4"></path></svg>
                                 </div>
                                 <span class="font-medium text-lg">Rosenbridge</span>
                             </div>
                        </div>
                    </div>
				</div>
			</Phone>
		</div>
	</Section>

	<!-- Meet Schema Divider -->
	<NavDivider active="Meet Schema" />

	<!-- Meet Schema Content -->
	<Section flip>
		<div slot="content" class="space-y-6">
			<h2 class="text-4xl md:text-5xl font-semibold tracking-tight text-gray-900 leading-tight">
				Meet Schema. A powerful new database client that fits in your pocket.
			</h2>
			<p class="text-lg text-gray-500 max-w-md leading-relaxed">
				Schema allows you to query and edit databases while you're away from your desk — giving you the flexibility of handling critical tasks quickly.
			</p>
		</div>
		<div slot="media">
			<Phone bgClass="bg-blue-500">
                <div class="flex flex-col h-full bg-white">
                    <!-- Header -->
                    <div class="bg-blue-500 text-white p-6 pt-12 pb-4">
                        <div class="text-2xl font-bold mt-4">SCHEMA</div>
                    </div>
                    <!-- List -->
                    <div class="p-4 space-y-4">
                        <div class="flex justify-between items-center border-b border-gray-100 pb-2">
                            <span class="font-semibold text-lg">Customers</span>
                            <span class="text-blue-500">Edit</span>
                        </div>
                        
                        <div class="space-y-2">
                            {#each ['ID', 'First Name', 'Last Name', 'Email', 'Phone', 'Company'] as label}
                            <div class="flex py-2 border-b border-gray-50">
                                <span class="w-1/3 text-gray-400 text-sm">{label}</span>
                                <span class="w-2/3 font-medium text-sm">...</span>
                            </div>
                            {/each}
                        </div>
                    </div>
                </div>
            </Phone>
		</div>
	</Section>

	<!-- Data Stored on Device -->
	<Section bgClass="bg-gray-50">
		<div slot="content" class="space-y-6">
			<h2 class="text-4xl md:text-5xl font-semibold tracking-tight text-gray-900">
				Data stored on device.
			</h2>
			<p class="text-lg text-gray-500 max-w-md leading-relaxed">
				Credentials are stored securely on your device and are never sent to our servers. We rely on iOS system protections to ensure your data is safe. We use FaceID/TouchID biometrics to lock access to the app for extra security.
			</p>
		</div>
		<div slot="media" class="relative">
            <!-- Abstract Illustration -->
            <div class="relative w-64 h-64">
                <!-- Blue shape -->
                <div class="absolute top-0 left-0 w-32 h-48 bg-blue-500 rounded-tr-[4rem] rounded-bl-[4rem]"></div>
                <!-- Yellow shape -->
                <div class="absolute bottom-0 right-10 w-24 h-32 bg-yellow-400 rounded-full flex items-center justify-center">
                     <div class="w-8 h-8 border-4 border-white rounded-full"></div>
                     <div class="w-2 h-6 bg-white absolute bottom-8"></div>
                </div>
                <!-- Red shape -->
                <div class="absolute top-10 right-0 w-16 h-16 bg-red-500 rounded-full"></div>
                <!-- Grid pattern overlay (simulated) -->
                <div class="absolute inset-0 bg-[url('data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjAiIGhlaWdodD0iMjAiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+PGNpcmNsZSBjeD0iMSIgY3k9IjEiIHI9IjEiIGZpbGw9IiNkMWQ1ZGIiLz48L3N2ZyA+')] opacity-30"></div>
            </div>
		</div>
	</Section>

	<!-- Databases Divider -->
	<NavDivider active="Databases" />

	<!-- Add Databases Quickly -->
	<Section bgClass="bg-white">
		<div slot="content" class="space-y-6">
			<h2 class="text-4xl md:text-5xl font-semibold tracking-tight text-gray-900 leading-tight">
				Add databases quickly. Connect to them directly.
			</h2>
			<p class="text-lg text-gray-500 max-w-md leading-relaxed">
				Add Postgres and MySQL databases quickly via URL or by entering connection details manually. Connect directly or via SSH tunnel.
			</p>
		</div>
		<div slot="media">
			<Phone bgClass="bg-yellow-400">
                 <div class="flex flex-col h-full bg-white m-4 rounded-[2rem] overflow-hidden shadow-sm">
                     <div class="bg-blue-500 h-32 p-6 flex flex-col justify-end">
                         <h3 class="text-white font-bold text-xl">SCHEMA</h3>
                     </div>
                     <div class="p-6 space-y-6">
                         <div class="space-y-1">
                             <div class="text-xs font-bold text-gray-400 uppercase">Name</div>
                             <div class="text-lg font-medium border-b border-gray-200 pb-1">App DB</div>
                         </div>
                         <div class="space-y-1">
                             <div class="text-xs font-bold text-gray-400 uppercase">Host</div>
                             <div class="text-lg font-medium border-b border-gray-200 pb-1">db.example.com</div>
                         </div>
                         <div class="space-y-1">
                             <div class="text-xs font-bold text-gray-400 uppercase">Port</div>
                             <div class="text-lg font-medium border-b border-gray-200 pb-1">5432</div>
                         </div>
                         <div class="space-y-1">
                             <div class="text-xs font-bold text-gray-400 uppercase">User</div>
                             <div class="text-lg font-medium border-b border-gray-200 pb-1">postgres</div>
                         </div>
                     </div>
                 </div>
            </Phone>
		</div>
	</Section>

	<!-- Meticulously Refined -->
	<Section flip>
		<div slot="content" class="space-y-6">
			<h2 class="text-4xl md:text-5xl font-semibold tracking-tight text-gray-900 leading-tight">
				Meticulously refined interface — a small gesture.
			</h2>
		</div>
		<div slot="media">
			<Phone>
                <div class="flex flex-col h-full bg-white pt-12">
                     <div class="px-6 pb-2 border-b border-gray-100 flex justify-between items-end">
                         <h3 class="text-3xl font-bold">Customers</h3>
                         <div class="text-blue-500 text-2xl mb-1">⌄</div>
                     </div>
                     <div class="flex-1 overflow-y-auto">
                         {#each ['James Smith', 'Maria Garcia', 'Robert Johnson', 'Michael Brown', 'William Davis', 'David Miller', 'Richard Wilson', 'Joseph Moore', 'Thomas Taylor', 'Charles Anderson'] as name}
                             <div class="px-6 py-4 border-b border-gray-50 flex justify-between items-center">
                                 <span class="font-medium text-gray-900">{name}</span>
                                 <span class="text-gray-300">›</span>
                             </div>
                         {/each}
                     </div>
                </div>
            </Phone>
		</div>
	</Section>

	<!-- Tables Start Simple -->
	<Section>
		<div slot="content" class="space-y-6">
			<h2 class="text-4xl md:text-5xl font-semibold tracking-tight text-gray-900 leading-tight">
				Tables start simple.
			</h2>
            <p class="text-lg text-gray-500 max-w-md leading-relaxed">
				A clean list view lets you scan your data. Sort and filter with ease to find exactly what you're looking for.
			</p>
		</div>
		<div slot="media">
			<Phone>
                 <div class="flex flex-col h-full bg-white pt-12">
                     <div class="px-6 pb-4 border-b border-gray-100">
                         <div class="flex items-center gap-2 text-gray-500 mb-2">
                             <span class="text-blue-500">‹</span>
                             <span>Tables</span>
                         </div>
                         <h3 class="text-3xl font-bold">Public.Users</h3>
                     </div>
                     <div class="flex-1">
                         {#each [1, 2, 3, 4, 5, 6, 7] as i}
                             <div class="px-6 py-3 border-b border-gray-50 flex gap-4">
                                 <div class="w-8 h-8 rounded-full bg-gray-100 flex items-center justify-center text-xs text-gray-500">{i}</div>
                                 <div class="flex-1 space-y-1">
                                     <div class="h-2 bg-gray-200 rounded w-3/4"></div>
                                     <div class="h-2 bg-gray-100 rounded w-1/2"></div>
                                 </div>
                             </div>
                         {/each}
                     </div>
                </div>
            </Phone>
		</div>
	</Section>

	<!-- A Table Setting for One -->
	<Section flip>
		<div slot="content" class="space-y-6">
			<h2 class="text-4xl md:text-5xl font-semibold tracking-tight text-gray-900 leading-tight">
				A table setting for one.
			</h2>
            <p class="text-lg text-gray-500 max-w-md leading-relaxed">
				Focusing on one record at a time allows for easier reading and editing. Tap any row to see the full details, formatted for the screen in your hand.
			</p>
		</div>
		<div slot="media">
			<Phone>
                 <div class="flex flex-col h-full bg-white pt-12">
                     <div class="px-6 pb-4 flex justify-between items-center border-b border-gray-100">
                         <div class="flex items-center gap-2 text-blue-500">
                             <span>‹</span>
                             <span>Customers</span>
                         </div>
                         <span class="font-semibold">Edit</span>
                     </div>
                     <div class="p-6 space-y-6">
                         {#each ['id', 'created_at', 'first_name', 'last_name', 'email', 'phone', 'company', 'role', 'active'] as field}
                             <div class="flex justify-between items-baseline border-b border-gray-50 pb-2">
                                 <span class="text-gray-400 text-sm font-medium">{field}</span>
                                 <span class="text-gray-900 font-medium">...</span>
                             </div>
                         {/each}
                     </div>
                </div>
            </Phone>
		</div>
	</Section>

	<!-- Formatting Section -->
	<div class="bg-yellow-400 py-24 px-6 md:px-12">
		<div class="max-w-7xl mx-auto grid grid-cols-1 md:grid-cols-2 gap-12 items-center">
			<div class="font-mono text-4xl md:text-5xl text-black/80 tracking-tighter">
				2 days ago
			</div>
			<div class="space-y-6">
				<h2 class="text-4xl md:text-5xl font-semibold tracking-tight text-black leading-tight">
					Formatting that makes data human-readable.
				</h2>
				<p class="text-lg text-black/70 max-w-md leading-relaxed">
					Dates, JSON, and other data types are formatted to be readable. Timestamps show relative time, JSON is pretty-printed, and booleans are clear toggles.
				</p>
			</div>
		</div>
	</div>

	<!-- Stay in Flow -->
	<Section bgClass="bg-white">
		<div slot="content" class="space-y-6">
			<h2 class="text-4xl md:text-5xl font-semibold tracking-tight text-gray-900 leading-tight">
				Stay in flow.
			</h2>
            <p class="text-lg text-gray-500 max-w-md leading-relaxed">
				With dark mode support and a clean interface, Schema fades into the background so you can focus on your data.
			</p>
		</div>
		<div slot="media">
			<Phone dark bgClass="bg-gray-900">
                 <div class="flex flex-col h-full bg-gray-900 text-white pt-12">
                     <div class="px-6 pb-4 border-b border-gray-800">
                         <h3 class="text-3xl font-bold">Orders</h3>
                     </div>
                     <div class="flex-1">
                         {#each [1, 2, 3, 4, 5, 6] as i}
                             <div class="px-6 py-4 border-b border-gray-800 flex justify-between items-center">
                                 <div class="space-y-1">
                                     <div class="w-32 h-3 bg-gray-700 rounded"></div>
                                     <div class="w-20 h-3 bg-gray-800 rounded"></div>
                                 </div>
                                 <div class="text-gray-600">›</div>
                             </div>
                         {/each}
                     </div>
                </div>
            </Phone>
		</div>
	</Section>

    <!-- Peaberry Section -->
    <Section bgClass="bg-white">
        <div slot="media">
             <Phone bgClass="bg-red-500">
                 <div class="flex flex-col h-full bg-white pt-12">
                     <div class="px-6 pb-2">
                         <div class="flex items-center gap-2 text-blue-500 mb-4">
                             <span>‹</span>
                         </div>
                         <h3 class="text-3xl font-bold mb-6">Peaberry ⌄</h3>
                         
                         <div class="space-y-1">
                             <div class="text-gray-400 text-sm font-bold uppercase mb-2">Tables</div>
                             {#each ['Customers', 'Accounts', 'Companies', 'Products', 'Subscriptions'] as item}
                                 <div class="flex justify-between items-center py-3 border-b border-gray-50">
                                     <div class="flex items-center gap-3">
                                         <div class="w-6 h-6 bg-gray-100 rounded flex items-center justify-center text-gray-400 text-xs">T</div>
                                         <span class="font-medium">{item}</span>
                                     </div>
                                     <span class="text-gray-400 text-sm">123</span>
                                 </div>
                             {/each}
                             <div class="pt-4 text-blue-500 text-sm font-medium">Table Folder (12)</div>
                         </div>
                     </div>
                 </div>
             </Phone>
        </div>
        <div slot="content" class="space-y-6">
             <h2 class="text-4xl md:text-5xl font-semibold tracking-tight text-gray-900 leading-tight">
                 Works even when your connection doesn't.
             </h2>
             <p class="text-lg text-gray-500 max-w-md leading-relaxed">
                 Schema caches your schema and data so you can browse tables and view records even when you're offline or have a spotty connection.
             </p>
        </div>
    </Section>

	<!-- Editing Divider -->
	<NavDivider active="Editing" />

    <!-- Editing Tags Visual -->
    <div class="bg-gray-50 py-24 overflow-hidden space-y-6">
        <!-- Row 1 -->
        <div class="flex gap-4 animate-scroll-left w-[200%]">
             {#each Array(20) as _, i}
                {#each ['PROD', 'STAGE', 'DEV', 'READ ONLY'] as tag}
                    <span class="px-6 py-2 rounded-full border-2 text-2xl font-bold whitespace-nowrap
                        {tag === 'READ ONLY' ? 'bg-yellow-400 border-yellow-400 text-black' : ''}
                        {tag === 'PROD' ? 'bg-gray-800 border-gray-800 text-white' : ''}
                        {tag === 'STAGE' ? 'border-gray-300 text-gray-400' : ''}
                        {tag === 'DEV' ? 'border-gray-300 text-gray-400' : ''}
                    ">
                        {tag}
                    </span>
                {/each}
             {/each}
        </div>
        <!-- Row 2 -->
        <div class="flex gap-4 animate-scroll-right w-[200%] -ml-[100%]">
             {#each Array(20) as _, i}
                {#each ['READ ONLY', 'PROD', 'STAGE', 'DEV'] as tag}
                    <span class="px-6 py-2 rounded-full border-2 text-2xl font-bold whitespace-nowrap
                        {tag === 'READ ONLY' ? 'bg-yellow-400 border-yellow-400 text-black' : ''}
                        {tag === 'PROD' ? 'bg-gray-800 border-gray-800 text-white' : ''}
                        {tag === 'STAGE' ? 'border-gray-300 text-gray-400' : ''}
                        {tag === 'DEV' ? 'border-gray-300 text-gray-400' : ''}
                    ">
                        {tag}
                    </span>
                {/each}
             {/each}
        </div>
    </div>

	<!-- Long-overdue SQL -->
	<Section>
		<div slot="content" class="space-y-6">
			<h2 class="text-4xl md:text-5xl font-semibold tracking-tight text-gray-900 leading-tight">
				A long-overdue SQL to the desktop client.
			</h2>
            <p class="text-lg text-gray-500 max-w-md leading-relaxed">
				Run raw SQL queries and view results with ease. A full-screen editor lets you write complex queries comfortably.
			</p>
		</div>
		<div slot="media">
			<Phone bgClass="bg-blue-500">
                 <div class="flex flex-col h-full bg-white pt-12">
                     <div class="px-6 pb-4 border-b border-gray-100">
                         <h3 class="text-2xl font-bold">KeyCustomers</h3>
                     </div>
                     <div class="flex-1 p-0">
                         {#each ['Select *', 'From users', 'Where active', '=', 'true', 'Order by', 'created_at', 'desc', 'Limit 10'] as line, i}
                             <div class="px-6 py-2 font-mono text-sm flex gap-4">
                                 <span class="text-gray-300 w-4 text-right">{i+1}</span>
                                 <span class="{['Select *', 'From users', 'Where active', 'Order by', 'Limit 10'].includes(line) ? 'text-blue-600 font-bold' : 'text-gray-800'}">{line}</span>
                             </div>
                         {/each}
                     </div>
                     <div class="bg-gray-50 p-4 border-t border-gray-200">
                         <div class="flex justify-between items-center">
                             <span class="text-xs text-gray-500">10 rows returned</span>
                             <div class="w-8 h-8 bg-blue-500 rounded-full flex items-center justify-center text-white">
                                 <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14.752 11.168l-3.197-2.132A1 1 0 0010 9.87v4.263a1 1 0 001.555.832l3.197-2.132a1 1 0 000-1.664z"></path><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 12a9 9 0 11-18 0 9 9 0 0118 0z"></path></svg>
                             </div>
                         </div>
                     </div>
                </div>
            </Phone>
		</div>
	</Section>

    <!-- Query Carefully -->
    <Section flip>
        <div slot="content" class="space-y-6">
            <h2 class="text-4xl md:text-5xl font-semibold tracking-tight text-gray-900 leading-tight">
                Query carefully.
            </h2>
            <p class="text-lg text-gray-500 max-w-md leading-relaxed">
                Schema warns you about destructive queries like DELETE or DROP before you run them, helping prevent accidental data loss.
            </p>
        </div>
        <div slot="media">
            <Phone>
                 <div class="flex flex-col h-full bg-white pt-12">
                     <div class="px-6 pb-4 border-b border-gray-100 flex justify-between items-center">
                         <span class="text-blue-500">Done</span>
                         <span class="font-bold">Query</span>
                         <span class="text-blue-500">Run</span>
                     </div>
                     <div class="flex-1 p-6 font-mono text-sm">
                         <div class="text-red-500 font-bold">DELETE FROM users</div>
                         <div class="text-gray-800">WHERE id = 123;</div>
                     </div>
                     <!-- Warning Toast Mockup -->
                     <div class="absolute bottom-10 left-6 right-6 bg-red-50 border border-red-100 rounded-xl p-4 shadow-lg">
                         <div class="flex gap-3">
                             <div class="text-red-500">
                                 <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 9v2m0 4h.01m-6.938 4h13.856c1.54 0 2.502-1.667 1.732-3L13.732 4c-.77-1.333-2.694-1.333-3.464 0L3.34 16c-.77 1.333.192 3 1.732 3z"></path></svg>
                             </div>
                             <div>
                                 <h4 class="font-bold text-red-900">Destructive Query</h4>
                                 <p class="text-xs text-red-700 mt-1">This query will delete data. Are you sure?</p>
                             </div>
                         </div>
                     </div>
                </div>
            </Phone>
        </div>
    </Section>

	<!-- Tools Divider -->
	<NavDivider active="Tools" />

    <!-- Share Table Rows -->
    <div class="relative overflow-hidden bg-blue-500 py-24">
        <!-- Concentric Circles Background -->
        <div class="absolute inset-0 flex items-center justify-center pointer-events-none">
            <div class="w-[800px] h-[800px] border-[40px] border-white/10 rounded-full absolute"></div>
            <div class="w-[600px] h-[600px] border-[40px] border-white/10 rounded-full absolute"></div>
            <div class="w-[400px] h-[400px] border-[40px] border-white/10 rounded-full absolute"></div>
            <div class="w-[200px] h-[200px] bg-yellow-400 rounded-full absolute"></div>
        </div>

        <div class="relative z-10 max-w-7xl mx-auto px-6 md:px-12 grid grid-cols-1 md:grid-cols-2 gap-12 items-center">
            <div class="flex justify-center">
                <Phone>
                    <div class="flex flex-col h-full bg-white pt-12">
                         <div class="px-6 pb-4 border-b border-gray-100">
                             <h3 class="text-2xl font-bold">Customers</h3>
                         </div>
                         <div class="p-6 space-y-4">
                             {#each ['Name', 'Email', 'Plan', 'Status', 'Renewal'] as label}
                                 <div class="space-y-1">
                                     <div class="text-xs text-gray-400 uppercase font-bold">{label}</div>
                                     <div class="h-4 bg-gray-100 rounded w-full"></div>
                                 </div>
                             {/each}
                         </div>
                         <!-- Share Sheet Mockup -->
                         <div class="absolute bottom-0 left-0 right-0 bg-white rounded-t-2xl shadow-[0_-10px_40px_rgba(0,0,0,0.1)] p-6 pb-12">
                             <div class="flex justify-between items-center mb-6">
                                 <span class="font-bold text-lg">Share Row</span>
                                 <div class="w-8 h-8 bg-gray-100 rounded-full flex items-center justify-center text-gray-500">✕</div>
                             </div>
                             <div class="flex gap-6 overflow-x-auto pb-2">
                                 <div class="flex flex-col items-center gap-2 min-w-[60px]">
                                     <div class="w-12 h-12 bg-green-500 rounded-xl flex items-center justify-center text-white">
                                         <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24"><path d="M.057 24l1.687-6.163c-1.041-1.804-1.588-3.849-1.587-5.946.003-6.556 5.338-11.891 11.894-11.891 3.181.001 6.167 1.24 8.413 3.488 2.245 2.248 3.481 5.236 3.48 8.414-.003 6.557-5.338 11.892-11.893 11.892-1.99-.001-3.951-.5-5.688-1.448l-6.305 1.654zm6.597-3.807c1.676.995 3.276 1.591 5.392 1.592 5.448 0 9.886-4.434 9.889-9.885.002-5.462-4.415-9.89-9.881-9.892-5.452 0-9.887 4.434-9.889 9.884-.001 2.225.651 3.891 1.746 5.634l-.999 3.648 3.742-.981zm11.387-5.464c-.074-.124-.272-.198-.57-.347-.297-.149-1.758-.868-2.031-.967-.272-.099-.47-.149-.669.149-.198.297-.768.967-.941 1.165-.173.198-.347.223-.644.074-.297-.149-1.255-.462-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.297-.347.446-.521.151-.172.2-.296.3-.495.099-.198.05-.372-.025-.521-.075-.148-.669-1.611-.916-2.206-.242-.579-.487-.501-.669-.51l-.57-.01c-.198 0-.52.074-.792.372-.272.297-1.04 1.017-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.095 3.2 5.076 4.487.709.306 1.263.489 1.694.626.712.226 1.36.194 1.872.118.571-.085 1.758-.719 2.006-1.413.248-.695.248-1.29.173-1.414z"/></svg>
                                     </div>
                                     <span class="text-xs">WhatsApp</span>
                                 </div>
                                 <div class="flex flex-col items-center gap-2 min-w-[60px]">
                                     <div class="w-12 h-12 bg-blue-500 rounded-xl flex items-center justify-center text-white">
                                         <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 12h.01M12 12h.01M16 12h.01M21 12c0 4.418-4.03 8-9 8a9.863 9.863 0 01-4.255-.949L3 20l1.395-3.72C3.512 15.042 3 13.574 3 12c0-4.418 4.03-8 9-8s9 3.582 9 8z"></path></svg>
                                     </div>
                                     <span class="text-xs">Messages</span>
                                 </div>
                                 <div class="flex flex-col items-center gap-2 min-w-[60px]">
                                     <div class="w-12 h-12 bg-gray-200 rounded-xl flex items-center justify-center text-gray-600">
                                         <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 16H6a2 2 0 01-2-2V6a2 2 0 012-2h8a2 2 0 012 2v2m-6 12h8a2 2 0 002-2v-8a2 2 0 00-2-2h-8a2 2 0 00-2 2v8a2 2 0 002 2z"></path></svg>
                                     </div>
                                     <span class="text-xs">Copy</span>
                                 </div>
                             </div>
                         </div>
                    </div>
                </Phone>
            </div>
            <div class="text-white space-y-6">
                <h2 class="text-4xl md:text-5xl font-semibold tracking-tight leading-tight">
                    Share table rows with an Expiring Link. Cut out the copy and paste.
                </h2>
                <p class="text-lg text-white/80 max-w-md leading-relaxed">
                    Share a secure, temporary link to a specific row. The recipient sees a beautifully formatted page, and you control how long they have access.
                </p>
            </div>
        </div>
    </div>

    <!-- Notifications keep tabs -->
    <Section>
        <div slot="content" class="space-y-6">
            <h2 class="text-4xl md:text-5xl font-semibold tracking-tight text-gray-900 leading-tight">
                Notifications keep tabs on tables — so you can close the tabs kept in your browser.
            </h2>
        </div>
        <div slot="media" class="flex items-center justify-center">
             <div class="bg-white p-6 rounded-2xl shadow-xl border border-gray-100 flex items-start gap-4 max-w-sm">
                 <div class="w-12 h-12 bg-blue-500 rounded-xl flex items-center justify-center text-white font-bold text-xl">S</div>
                 <div>
                     <div class="font-bold text-gray-900">New Customer Row</div>
                     <div class="text-gray-500 text-sm mt-1">A row was recently inserted in Shell Space.</div>
                 </div>
             </div>
        </div>
    </Section>

    <!-- Search across multiple tables -->
    <Section bgClass="bg-gray-50">
        <div slot="media" class="relative min-h-[400px]">
             <!-- Grid Background -->
             <div class="absolute inset-0 bg-[url('data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDAiIGhlaWdodD0iNDAiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+PHBhdGggZD0iTTAgMGg0MHY0MEgwVjB6bTEgMWgzOHYzOEgxVjF6IiBmaWxsPSIjZTVlN2ViIiBmaWxsLXJ1bGU9ImV2ZW5vZGQiLz48L3N2Zz4=')] opacity-50"></div>
             
             <!-- Search UI Mockup -->
             <div class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 w-full max-w-md px-6">
                 <div class="bg-white rounded-xl shadow-lg p-2 flex items-center gap-3 border border-gray-200">
                     <Search class="w-6 h-6 text-gray-400 ml-2" />
                     <span class="text-xl text-gray-400 font-light">Search...</span>
                 </div>
             </div>
        </div>
        <div slot="content" class="space-y-6">
            <h2 class="text-4xl md:text-5xl font-semibold tracking-tight text-gray-900 leading-tight">
                Search across multiple tables. Find what you need, even when you're not sure where to look.
            </h2>
        </div>
    </Section>

	<!-- Footer -->
	<footer class="bg-blue-500 py-32 px-6 text-center text-white">
		<div class="max-w-xl mx-auto space-y-8">
			<h2 class="text-3xl md:text-4xl font-bold">Available on the App Store</h2>
			<Button variant="white">
				<Apple class="w-5 h-5" />
				<span>Download</span>
			</Button>
		</div>
	</footer>
</div>

<style>
    /* Custom scrollbar for phone mockups */
    ::-webkit-scrollbar {
        width: 0px;
        background: transparent;
    }
</style>

