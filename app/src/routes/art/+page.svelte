<script lang="ts">
  import Gallery from "./Gallery.svelte";
  import type { Piece } from "./pieces";

  const pieces: Piece[] = [
    { name: 'Good Technique', img: '/art/good-technique.png', pdf: '/art/good-technique.pdf' },
    { name: 'Slow is Smooth, Smooth is Fast', img: '/art/slow-is-smooth.png', pdf: '/art/slow-is-smooth.pdf' },
    { name: 'Just Get Shit Done', img: '/art/just-get-shit-done.png', pdf: '/art/just-get-shit-done.pdf' },
    { name: 'Brick Check', img: '/art/brick-check.png', pdf: '/art/brick-check.pdf' },
  ]
</script>

<style>
  .container {
    padding: 2rem;
    height: 100vh;
  }

  .main-link {
    display: inline-block;
    margin-bottom: 1.5rem;
    font-size: 1.5rem;
    text-decoration: none;
    color: #00f260;
    font-weight: bold;
    border-bottom: 2px solid transparent;
    transition: border-color 0.3s, color 0.3s;
  }

  .main-link:hover {
    border-color: #00f260;
    color: #0575e6;
  }
</style>

<div class="container">
  <a href=".." class="main-link">Tribulnation</a>
  <Gallery {pieces} />
</div>
