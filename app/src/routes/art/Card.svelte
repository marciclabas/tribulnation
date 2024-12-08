<script lang="ts">
  import type { Piece } from "./pieces";
  const piece: Piece = $props()
</script>

<style>
  .card {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
    text-align: center;
    background: #1f1f1f;
    border-radius: 12px;
    overflow: hidden;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    transition: transform 0.2s ease-in-out;
    padding: 1rem;
  }

  .card:hover {
    transform: translateY(-5px);
    box-shadow: 0 6px 12px rgba(0, 0, 0, 0.3);
  }

  img {
    width: 100%;
    object-fit: cover;
    border-radius: 8px;
  }

  h3 {
    font-size: 1.2rem;
    color: #fff;
    margin: 0.5rem 0;
    text-transform: uppercase;
  }

  a { 
    color: #fff;
    text-decoration: none;
    background: #333;
    padding: 0.5rem 1rem;
    border-radius: 8px;
    transition: all 0.2s ease-in-out;
  }

  a:hover {
    background: #555;
  }

</style>

<div class="card">
  <img src={piece.img} alt={piece.name} />
  <h3>{piece.name}</h3>
  <a href={piece.pdf}>PDF</a>
</div>
