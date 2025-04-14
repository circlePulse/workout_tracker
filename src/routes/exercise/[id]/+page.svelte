<script>
	import { page } from '$app/stores';

	// Grab the dynamic route ID (like "squat")
	$: id = $page.params.id;
</script>

<h1 class="text-2xl font-semibold mb-2">Exercise: {id}</h1>
<p>This is where you'll see graphs, workout entries, and a form for {id}.</p>
