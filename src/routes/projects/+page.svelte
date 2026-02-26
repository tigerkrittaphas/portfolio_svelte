<svelte:head>
  <title>Projects</title>
</svelte:head>

<script>
  import projects from "$lib/projects.json";
  import Project from "$lib/Project.svelte";
</script>

<h1>My Projects</h1>

<h2>I have {projects.length} projects</h2>

<div class="projects">
  {#each projects as p}
    <Project data={p} />
  {/each}
</div>
