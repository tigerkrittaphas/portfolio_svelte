<script>
    export let data = {};
</script>

<article>
    <img src={data.image} alt={data.title} />
    <div class="meta">
        <h3>{data.title}</h3>
        <p>{data.author}</p>
    </div>
</article>  


<style>
:global(.readings) {
    display: flex;
    flex-direction: column;
    gap: 0.9rem;
}

img {
    width: clamp(58px, 9vw, 84px);
    aspect-ratio: 1 / 1;
    object-fit: cover;
    border-radius: 0.7rem;
    border: 1px solid oklch(86% 0.02 220);
    flex-shrink: 0;
}

article {
    display: flex;
    align-items: center;
    gap: 1rem;
    padding: 0.9rem 1rem;
    border: 1px solid oklch(85% 0.02 230);
    border-radius: 0.9rem;
    background: linear-gradient(120deg, oklch(98% 0.01 250), oklch(96% 0.01 210));
    box-shadow: 0 8px 16px oklch(30% 0.02 240 / 0.08);
    transition: transform 160ms ease, box-shadow 160ms ease;
}

article:hover {
    transform: translateY(-2px);
    box-shadow: 0 12px 22px oklch(30% 0.03 240 / 0.14);
}

.meta {
    display: flex;
    flex-direction: column;
    gap: 0.2rem;
    min-width: 0;
}

h3 {
    margin: 0;
    line-height: 1.2;
    font-size: 1.05rem;
}

p {
    margin: 0;
    color: oklch(44% 0.03 250);
}

@media (max-width: 640px) {
    article {
        align-items: flex-start;
        padding: 0.8rem 0.9rem;
    }
}
</style>
