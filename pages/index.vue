<template>
  <div class="container">
    <header>
      <div class="logo">
        <h1>Francesco Scheffczyk</h1>
        <h2>– Laboratory</h2>
      </div>

      <a href="mailto:francesco.scheffczyk@outlook.com">Contact</a>
    </header>

    <main>
      <p class="social">
        <a href="https://www.instagram.com/francesco.scheffczyk/">ig</a>
        –
        <a href="https://www.linkedin.com/in/francesco-scheffczyk/">li</a>
        –
        <a href="https://github.com/Francesco-Sch">gh</a>
      </p>

      <div class="marquee">
        <div class="track">
          Coming Soon Coming Soon Coming Soon Coming Soon
        </div>
      </div>
    </main>
  </div>
</template>

<script>
export default {
  name: 'ComingSoon',
}
</script>

<style lang="scss" scoped>
.container {
  width: 100%;
  height: 100%;

  padding: 3.5%;

  background-color: black;
  color: white;

  a {
    color: white;
    text-decoration: none;

    padding: 5px;

    &:hover {
      text-decoration: underline;
    }
  }

  header {
    display: flex;
    flex-direction: row;
    justify-content: space-between;

    width: 100%;

    h1 {
      font-family: 'Fracktif Medium', Arial, Helvetica, sans-serif;
      font-size: 1.75em;
      font-weight: 400;
      margin: 0;
    }
    h2 {
      font-family: 'Fracktif Medium', Arial, Helvetica, sans-serif;
      font-size: 1.75em;
      font-weight: 400;
      margin: 0;
    }
  }

  main {
    display: flex;
    flex-direction: row-reverse;
    align-items: center;
    height: 80%;

    .social {
      transform: rotate(90deg) translateY(-225%);
    }
  }

  .marquee {
    position: absolute;
    bottom: 0;
    left: 0;
    height: 45vh;
    width: 100%;
    overflow: hidden;

    font-family: 'Fracktif Medium', Arial, Helvetica, sans-serif;
    font-size: 45vh;

    .track {
      white-space: nowrap;
      will-change: transform;
      animation: marquee 15s linear infinite;

      color: transparent;
      -webkit-text-stroke: 1px white;
    }

    @keyframes marquee {
      from {
        transform: translateX(0);
      }
      to {
        transform: translateX(-173%);
      }
    }
  }
}
</style>
