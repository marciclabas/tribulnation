<script>

    import { base } from "$app/paths";

</script>
<div class="landing">
  <h1>Tribulnation</h1>
  <p>Who are we? We make shit happen.</p>
  <a href={`${base}/art`} class="neon-border">Explore More</a>
</div>

<style>
  .landing {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background: linear-gradient(135deg, #0f0c29, #302b63, #24243e);
    color: white;
    text-align: center;
  }

  h1 {
    font-size: 4rem;
    font-weight: 900;
    text-transform: uppercase;
    letter-spacing: 0.1em;
    background: linear-gradient(90deg, #00f260, #0575e6);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    margin-bottom: 1rem;
  }

  p {
    font-size: 1.5rem;
    font-weight: 300;
    color: #dcdcdc;
    max-width: 600px;
    line-height: 1.8;
    margin-top: 0;
  }

  .neon-border {
    margin-top: 2rem;
    padding: 0.8rem 2rem;
    border: 2px solid #00f260;
    border-radius: 30px;
    text-transform: uppercase;
    letter-spacing: 0.15em;
    color: #00f260;
    cursor: pointer;
    transition: all 0.3s ease-in-out;
    font-size: 1rem;
  }

  .neon-border:hover {
    background: #00f260;
    color: #24243e;
  }

  a {
    text-decoration: none;
  }
</style>
