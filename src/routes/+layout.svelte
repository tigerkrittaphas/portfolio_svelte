<script>
	import { base } from '$app/paths';
</script>

<nav>
	<a href={`${base}/`}>Home</a>
	<a href={`${base}/projects/`}>Projects</a>
	<a href={`${base}/resume/`}>Resume</a>
	<a href={`${base}/contact/`}>Contact</a>
	<a href="https://github.com/tigerkrittaphas" target="_blank" rel="noopener noreferrer">GitHub</a>
</nav>

<slot />
