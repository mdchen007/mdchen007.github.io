<script lang="ts">
    let category = $state('default');
</script>


<h1>Blog</h1>
<a href="/">Back</a>
<br>
<button onclick={() => {category='default'}}>預設</button>
<button onclick={() => {category='hiking'}}>爬山</button>

{#if category == 'default'}
<h2>blog 1</h2>
<p>adspfoidsajfposaf</p>
{/if}

{#if category == 'default'}
<h2>blog 2</h2>
<p>adspfoidsajfposaf</p>
{/if}

{#if category == 'default' || category == 'hiking'}
<h2>blog 3</h2>
<p>adspfoidsajfposaf 爬山</p>
{/if}