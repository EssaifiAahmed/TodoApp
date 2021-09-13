<script>
	import  Header  from "./components/header.svelte";
	import  List  from "./components/List.svelte";
</script>


<style>
	.container{
		width: 500px;
	}
	:global(.container *) {
		font-family: "Quicksand", sans-serif;
		background-color: #009579;
	}
</style>

<dev class="container">
	<Header />
	<List />
</dev>