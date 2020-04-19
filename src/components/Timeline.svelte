<script>
  import Card from "./Card.svelte";

  export let posts = [];
</script>

<style>
  .Timeline {
    padding: 4em 0 0 0;
  }
</style>

<div class="Timeline">
  <div class="timeline-container">
    {#each posts as post}
      <Card {...posts} />
    {:else}
      <p>Loading...</p>
    {/each}
  </div>
</div>

<!-- TimeLine.svelte -->
