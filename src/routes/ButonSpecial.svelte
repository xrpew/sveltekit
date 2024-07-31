<script>
    	const handleclick = (e) =>{
        e.target.disabled=true
		e.target.innerText='⭐'
	}
</script>


<button on:click={ handleclick}
class="inline-flex items-center justify-center hover:backdrop-brightness-50 whitespace-nowrap rounded-md text-sm font-medium ring-offset-background transition-colors focus-visible:outline-none focus-visible:ring-2 focus-visible:ring-ring focus-visible:ring-offset-2 disabled:pointer-events-none disabled:opacity-50 border border-input bg-background hover:bg-accent hover:text-accent-foreground h-10 px-4 py-2"
>
Me gusta :)
</button>