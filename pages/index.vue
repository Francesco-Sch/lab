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
      <p>
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

    a {
      color: white;
      text-decoration: none;

      &:hover {
        text-decoration: underline;
      }
    }
  }
}
</style>
