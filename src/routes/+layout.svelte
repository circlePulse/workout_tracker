<script>
	import '../app.css';
	import { House } from 'lucide-svelte';

	let { children } = $props();
</script>
<nav class="bg-gray-100 p-4 mb-4">
	<House />
	<a class="mr-4" href="/">Dashboard</a>
</nav>
{@render children()}



