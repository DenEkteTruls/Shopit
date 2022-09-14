<script>
	import router from 'page';

	import Login from './Login.svelte';
	import Home from './Home.svelte';

	let page = Home;

	router("/", () => page = Home);
	router("/login", () => page = Login);

	router.start();
</script>


<svelte:component this={page}/>


<!-- INSPO: https://dribbble.com/shots/15191201-Groceries-Cart-Shopping-List/attachments/6934177?mode=media -->