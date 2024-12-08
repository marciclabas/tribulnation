<script lang="ts" module>
  export type Props = {
    pieces: Piece[]
  }

</script>

<script lang="ts">
  import Card from './Card.svelte';
  import type { Piece } from './pieces';
  const { pieces }: Props = $props()
</script>

<style>
  div {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 1.5rem;
    background: #121212;
  }
</style>

<div>
  {#each pieces as piece}
    <Card {...piece} />
  {/each}
</div>
