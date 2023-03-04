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
  align-items: center;
  grid-template-columns: 1fr 1fr;
  grid-gap: 2rem; /* add a gap between the grid columns */
}

section {
  height: 450px;
  flex-direction: column;
  align-items: center;
}

.content-main {
  line-height: 1;
  align-items: center; /* center the content horizontally */
  text-transform: capitalize;
  padding: 2rem; /* add some padding to the section */
   /* center the text horizontally */
}

.content-main h1 {
  font-size: 49px;
  
}

.content-main h2 {
  font-size: 29px;
}

.content-img img {
  width: 85%;
  height: auto;
}

.buttons {
  margin-top: 1rem;
  gap: 1rem;
  display: flex; /* add display flex to align buttons horizontally */
  justify-content: center; /* center the buttons horizontally */
}

.btn {
  padding: 0.5rem 0.9rem;
}

@media only screen and (max-width: 650px) {
  main {
    margin: 0 auto;
    grid-template-columns: 1fr; /* change to a single column grid */
    grid-gap: 1rem; /* reduce the gap between the grid items */
    justify-content: center; /* center the grid items horizontally */
  }

  section {
    height: auto; /* remove fixed height to fit content */
  }

  .content-main {
   /* padding: 1rem; */
    align-items: center;    
  }

  .content-main h1 {
    font-size: 35px;
  }

  .content-main h2 {
    font-size: 19px;
    
  }

  .content-img {
    justify-content: center;
  }

  .content-img img {
    width: 100%;
  }

  .buttons {
    margin-top: 1rem;
    gap: 1rem;
    
    align-items: center; /* center the buttons horizontally */
  }
}

</style>