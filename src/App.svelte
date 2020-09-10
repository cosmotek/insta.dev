<script>
	import TextField from './TextField.svelte';
	import Button from './Button.svelte';
	import MIOBanner from './MIOBanner.svelte';

	export let name;
</script>

<main>
	<h1>Hello {name}!</h1>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>

	<div id="abc">
		<TextField label="First Name" placeholder="John"/>
		<TextField label="Last Name" placeholder="Smith"/>
	</div>

	<Button text="Create" onTap={() =>console.log(Math.random())}/>

	<MIOBanner/>
</main>

<style lang="scss" global>
	@import "./fonts.scss";
	@import "./colors.scss";

	h1, h2, h3, p, a, li, ul, button, input {
		/* font-family: 'GilroyLight', sans-serif; */
		font-family: 'Gilroy', sans-serif;
		color: $th-txt-dark;
	}

	a {
		color: $th-primary;
		font-weight: 700;
	}
</style>
