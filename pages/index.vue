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
        <a href="">ig</a>
        –
        <a href="">li</a>
        –
        <a href="">gh</a>
      </p>

      <div class="marquee">
        <p>Coming Soon</p>
      </div>
    </main>
  </div>
</template>

<script>
export default {}
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
      margin: 0;
    }
    h2 {
      font-family: 'Fracktif Medium', Arial, Helvetica, sans-serif;
      font-size: 1.75em;
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
    height: 30vh;
    width: 100%;
  }
}
</style>
