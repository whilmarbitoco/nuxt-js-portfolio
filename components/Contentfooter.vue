<template>
        <div class="container">
        <footer>
          <nuxt-img src="down-icon.png" />
        </footer>
        </div>
</template>

<script>
export default {
  name: 'Contentfooter'
};
</script>

<style scoped>
  footer { 
    display: flex;
    align-items: center;
    justify-content: center;
  }
footer img {
  width: 24px;
  margin-bottom: 5rem;
  cursor: pointer;
  }
</style>
