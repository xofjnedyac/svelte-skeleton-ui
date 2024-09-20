<script>
	import MyButton from "./Button.svelte";
	import Popcard from "./Popcard.svelte";
</script>

<svelte:head>
<link rel="stylesheet" href="https://unpkg.com/tailwindcss@2.2.19/dist/tailwind.min.css"/>
</svelte:head>


<div class="flex flex-row space-x-4 p-4 bg-blue-50">
<Popcard type="dark"/>
<Popcard type="light"/>
</div>