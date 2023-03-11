<template>
    <div id="project" class="container">
            <header>
                <h1>Projects</h1>
                <p>Here's some projects that I have done.</p>
            </header>
    <Project :list="list" />
    </div>
</template>

<script>
import axios from 'axios'
export default {
  name: 'Projects',
  data() {
    return {
      list: []
    }
  },
  
  async created() {
    const response = await axios.get("https://jsonplaceholder.typicode.com/users")
    this.list = response.data
    }
  }

  
</script>

<style scoped>
img {
    width: 100%;
    height: 100%;
}

a {
    text-decoration: none;
    color: inherit;
}

header {
    margin: 1rem;
}

h1 {
    font-size: 2.5rem;
    text-align: center;
    margin-top: 2rem;
    margin-bottom: 1rem;
    color: #444;
}

p {
    text-align: center;
    margin-bottom: 2rem;
    color: #777;
    font-size: 0.9rem;
}

.container {
    width: 100vw;
  margin: 0 auto;
   /* background-color: #f7f7f7;*/
}

</style>