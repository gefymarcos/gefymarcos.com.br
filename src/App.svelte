<script lang="ts">
  import githubLogo from './assets/github.svg'
  import code4tubaLogo from './assets/code4tuba.png'
</script>

<main>
  <div>
    <h1>@gefymarcos</h1>
    <a href="https://code4tuba.com.br" target="_blank" rel="noreferrer"> 
      <img src="{code4tubaLogo}" class="logo code4tuba" alt="Code4tuba Logo" />
    </a>
    <a href="https://github.com/gefymarcos" target="_blank" rel="noreferrer"> 
      <img src={githubLogo} class="logo github" alt="Github Logo" />
    </a>
  </div>
</main>

<style>
  .logo {
    height: 7em;
    padding: 1.5em;
    will-change: filter;
  }
  .logo:hover {
    filter: drop-shadow(0 0 2em #646cffaa);
  }
  .logo.github:hover {
    filter: drop-shadow(0 0 2em #fff1f1aa);
  }
</style>