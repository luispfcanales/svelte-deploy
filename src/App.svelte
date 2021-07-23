<script>
	import { Router, Route, Link } from "svelte-routing"
</script>

<Router basepath="/svelte-deploy">
	<nav>
		<Link to="/">Home</Link>
		<Link to="about">About</Link>
	</nav>

	<main>
		<Route path="/">
			<h3>Home Route</h3>
		</Route>

		<Route path="about">
			<h3>About Route</h3>
		</Route>
		<Route path="*">
			<h3>error</h3>
		</Route>
	</main>
</Router>

<style>
	h3 {
		color:darkslateblue;
	}
</style>
