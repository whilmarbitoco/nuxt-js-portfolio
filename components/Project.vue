<template>
  <div class="card-container">
    <div v-for="l in list" :key="l.id" class="card">
      <div class="card-image">
        <img src="test.jpg" alt="project preview" />
      </div>
      <div class="card-info">
        <h2 class="card-title">{{ l.name }}</h2>
        <p class="card-description">
          A {{ l.company.bs }}
        </p>
      </div>
      <div class="card-actions">
        <a href="#" class="card-action">
          <font-awesome-icon icon="eye" class="card-icon" />
          Demo
        </a>
        <a href="#" class="card-action">
          <font-awesome-icon icon="code" class="card-icon" />
          Code
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Project",
  props: {
    list: Array,
  },
};
</script>

<style>
.card-container {
  margin: 2rem;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  grid-template-rows: auto;
  gap: 2rem;
}

.card {
  font-family: "Roboto", sans-serif;
  width: 100%;
  height: 400px;
  border-radius: 5px;
  border: 1px solid #ddd;
  overflow: hidden;
  position: relative;
  background-color: #fff;
  box-shadow: 0px 5px 10px rgba(0, 0, 0, 0.2);
  transition: box-shadow 0.3s ease-in-out;
}

.card:hover {
  box-shadow: 0px 10px 20px rgba(0, 0, 0, 0.3);
}

.card-image {
  width: 100%;
  height: 60%;
  overflow: hidden;
  position: relative;
}

.card-image img {
  object-fit: cover;
  height: 100%;
  width: 100%;
  transition: transform 0.5s ease;
}

.card:hover .card-image img {
  transform: scale(1.1);
}

.card-info {
  margin: 1rem;
}

.card-title {
  font-size: 1.5rem;
/*  margin-bottom: 0.5rem;*/
}

.card-description {
  font-size: 0.8em;
  color: #777;
}

.card-actions {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 1rem;
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 60px;
  background-color: #f5f5f5;
  border-top: 1px solid #ddd;
}

.card-action {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  color: #444;
  font-size: 1.1rem;
  text-decoration: none;
}

.card-action:hover {
  color: #000;
}

.card-icon {
  font-size: 1.2rem;
}
</style>
