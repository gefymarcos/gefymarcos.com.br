<script lang="ts">
  import githubLogo from "./assets/github.svg";
  import gmailLogo from "./assets/gmail.svg";
  import twitterLogo from "./assets/twitter.svg";
  import linkedinLogo from "./assets/linkedin.svg";
  import code4tubaLogo from "./assets/code4tuba.svg";
  const title = `Olá humano!`;
  const style = (index) => {
    return 0 + index / 13 + "s";
  };
</script>

<main>
  <div>
    <h1>
      {#each title as char, i}
        <span aria-hidden="true" style="animation-delay: {style(i + 8)};">
          {#if char}
            {char}
          {/if}
          {#if i === 3}
            <span>&nbsp;</span>
          {/if}
        </span>
      {/each}
      <span class="cursor" />
    </h1>

    <a href="https://twitter.com/gefymarcos" target="_blank" rel="noreferrer">
      <img src={twitterLogo} class="logo github" alt="Github Logo" />
    </a>
    <a href="https://github.com/gefymarcos" target="_blank" rel="noreferrer">
      <img src={githubLogo} class="logo github" alt="Github Logo" />
    </a>
    <a
      href="mailto:gefymarcos@gmail.com"
      target="_blank"
      rel="noreferrer"
      title="Email"
    >
      <img src={gmailLogo} class="logo github" alt="Github Logo" />
    </a>
    <a
      href="https://linkedin.com/in/geffersonmarcos"
      target="_blank"
      rel="noreferrer"
    >
      <img src={linkedinLogo} class="logo github" alt="Github Logo" />
    </a>
    <a href="https://code4tuba.com.br" target="_blank" rel="noreferrer">
      <img src={code4tubaLogo} class="logo code4tuba" alt="Code4tuba Logo" />
    </a>
  </div>
</main>

<style>
  .logo {
    height: 2rem;
    padding: 1rem;
    will-change: filter;
  }
  .logo:hover {
    filter: drop-shadow(0 0 2em #646cffaa);
  }
  .logo.github:hover {
    filter: drop-shadow(0 0 2em #fff1f1aa);
  }
</style>
