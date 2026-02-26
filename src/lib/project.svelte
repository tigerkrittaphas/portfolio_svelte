<script>
    export let data = {};
</script>

<article>
    <h2>{data.title}</h2>
    <img src={data.image} alt="" />
    <p>{data.description}</p>
</article>  


<style>
img {
	max-width: 100%;
}

article {
	grid-template-rows: subgrid;
	grid-row: span 3;
}
</style>