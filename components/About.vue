<template>
  <div class="container">
    <h2>About Me</h2>
    <div class="section-container">
      <section class="one">
        <div class="img-container">
          <img src="coding.png" alt="A photo of me" />
        </div>
      </section>
      <section class="two">
        <h3>Who am I?</h3>
        <p>
          Hi there! My name is Whilmar Bitoco, and I'm a Web Developer. I'm passionate about technology and have been developing my skills in programming. In my free time, I enjoy reading and drinking coffee.
        </p>
        
        <div class="skills">
          <h3>My Skills</h3>
          <ul>
            <skill-item skill="HTML" progress="80%" />
            <skill-item skill="CSS" progress="75%" />
            <skill-item skill="JavaScript" progress="60%" />
            <skill-item skill="Vue.js" progress="80%" />
            <skill-item skill="Express.js" progress="70%" />
            <skill-item skill="SQLITE" progress="65%" />
          </ul>
        </div>
      </section>
    </div>
  </div>
</template>

<script>
export default {
  name: 'About',
  
}
</script>

<style scoped>
  img {
    width: 100%;
    /*height: 100%;*/
}

.container {
    margin: 1rem;
}

h2 {
    text-align: center;
}

.section-container {
    /* background: #f2f2f2; */
    width: 90vw;
    margin: 0 auto;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

section {
    width: 50%;
    padding: 1rem;
}

.two p {
    padding: 1rem;
}

.skills {
    margin-top: 2rem;
}

@media screen and (max-width: 550px) {
    .section-container {
        flex-direction: column;
    }
    section {
        width: 100%;
    }
}

</style>
