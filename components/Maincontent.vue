<template>
  <div class="container">
    <main>
      <section class="content-main">
        <h2>Hello, I am</h2>
        <h1>Whilmar Bitoco</h1>
        <p>A 17 Year Old Frond-End Web Developer from the philippines</p>
        <div class="buttons">
          <a href="#" class="btn">Download CV</a>
          <a href="#" class="btn">Portfolio</a>
        </div>
      </section>
      <section class="content-img">
        <nuxt-img src="person.svg" />
      </section>
    </main>
  </div>
</template>

<script>
export default {
  name: 'Maincontent'
};
</script>

<style scoped>
.container {
  max-width: 75rem;
  width: 100%; /* added */
  margin: 0 auto;
}
  
main {
  display: grid;
  grid-template-columns: 1fr 1fr;
}

section,
.container footer,
.buttons {
  display: flex;
  justify-content: center;
}

section {
  height: 450px;
  flex-direction: column;
  align-items: center;
}

.content-main {
  line-height: 1;
  align-items: flex-start;
  padding-left: 9rem;
  text-transform: capitalize;
}

.content-main h1 {
  font-size: 3.5rem; /* changed to relative unit */
}

.content-main h2 {
  margin-left: 0;
}

.content-img img {
  width: 85%;
  max-width: 100%; /* added */
}

.buttons {
  margin-top: 1rem;
  gap: 1rem;
}

@media only screen and (max-width: 650px) {
  main {
    justify-content: space-around;
    margin: 0 auto;
    grid-template-columns: 1fr;
    
  }

  .content-main {
    align-items: center;
    padding: 2rem; /* added */
  }

  .content-main h1 {
    font-size: 2.3rem;
  }

  .content-main h2 {
    align-self: flex-start;
    font-size: 1.2rem;
  }

  .content-img img {
    display: none;
  }
}
</style>
