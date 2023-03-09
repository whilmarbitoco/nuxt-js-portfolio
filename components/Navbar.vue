<template>
      <div class="container">
        <nav>
          <div class="logo">
            <nuxt-img src="/coding.png" />

            <h1>Whilmar Bitoco</h1>
          </div>
          <div class="links">
            <a href="#" class="link">Home</a>
            <a href="#project" class="link">Portfolio</a>
            <a href="#" class="link">About</a>
            <a href="#" class="link btn">Contact</a>
          </div>
        </nav>
      </div>
</template>

<script>
export default {
  name: 'Navbar',
}
</script>

<style scoped>
.logo {
  display: flex;
  align-items: center;
  justify-content: center;
}

.logo img {
  width: 40px;
}

a {
  text-decoration: none;
  }

a:hover {
  color: #56b4c9;
  border-bottom: 1px solid #56b4c9;
}

.btn:hover {
  color: #FFF;
}

  nav {
  margin-top: 1rem;
  padding: 1rem;
}

nav .links {
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 1rem;
}

  @media (max-width: 550px) {
  .container {
    width: 100%;
  }
    
  nav .logo h1 {
    display: none;
  }

  nav a {
    font-size: 13px;
  }

  nav .links {
    gap: 10px;
  }
}


</style>
