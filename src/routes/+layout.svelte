<script>
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';
	
	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>


<div class="navbar bg-base-100 shadow-sm">
	<div class="flex-1">
		<a class="btn btn-ghost text-xl">Empresa</a>
	</div>

	<div class="flex-none">
	
		<ul class="menu menu-horizontal px-1">
			<li><a>Link</a></li>
			<li>	
				<details>
					<summary>Menu</summary>
					<ul class="bg-base-100 rounded-t-none p-2">
						<li><a>Link 1</a></li>
						<li><a>Link 2</a></li>
					</ul>
				</details>
			</li>
		</ul>
	
	</div>
</div>



{@render children()}
