<script>
  import projects from "$lib/projects.json";
  import Project from "$lib/Project.svelte";
  import readings from "$lib/readings.json";
  import ReadingItem from "$lib/readingItem.svelte";
</script>

<h1>Tiger Chai</h1>

<p>Showing my personal information. This is try to type the paragraph to be so long so it crash with the page border. This is try to type the paragraph to be so long so it crash with the page border.</p>

<img src="images/my_image.jpeg" alt="Figure 1: CORGI!!" height="300">

<h2> Latest Projects </h2>

<div class="projects">
    {#each projects.slice(0, 3) as p}
        <Project data={p} />
    {/each}
</div>

<h2> I'm Reading </h2>

<div class="readings">
    {#each readings.slice(0,3) as r}
        <ReadingItem data={r} />
    {/each}
</div>