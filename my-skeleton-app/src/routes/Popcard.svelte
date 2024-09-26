<script>
    import MyButton from "./Button.svelte";
        export let decline = "No, thanks";
        export let image = "https://media.rainpos.com/11419/ikidhimase_seuqhoehaw8_unsplash.jpg";
        export let message = "Introducting Virtual Reality";
        export let subhead ="Please check out all-new feature";
        export let type = "light";
        export let color = "purple";
        
    </script>
    
    {#if type==="light"}
    <div class="w-80 h-3/4 bg-gray-50  flex-col space-y-1 rounded-xl pb-4 shadow-md">
        <img src="{image}" alt="card" class="mb-5 h-48 w-full object-cover rounded-t-lg">
        <h1 class="text-center text-gray-900 text-3xl font-bold">{message}</h1>
        <h2 class="text-center text-gray-500 pt-2 p-5 text-md">{subhead}</h2>
        <MyButton name="Sure" color="{color}"/>
        <p class="text-{color}-700 text-center pt-2"><a href="/index.html">{decline}</a></p>
    </div>
    {/if}
    
    {#if type==="dark"}
    <div class="w-80 h-3/4 bg-gray-800  flex-col space-y-1 rounded-xl pb-4 shadow-md">
        <img src="{image}" alt="card" class="mb-5 h-48 w-full object-cover rounded-t-lg">
        <h1 class="text-center text-gray-50 text-3xl font-bold">{message}</h1>
        <h2 class="text-center text-gray-300 pt-2 p-5 text-md">{subhead}</h2>
        <MyButton name="Sure" color="{color}"/>
        <p class="text-gray-400 text-center pt-2"><a href="/index.html">{decline}</a></p>
    </div>
    {/if}