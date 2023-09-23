<script>
  export let data;
</script>

<h1>Journal</h1>

<ul>
  {#each data.summaries as {slug, title} }
    <li><a href="/journal/{slug}">{title}</a></li>
  {/each}
</ul>
