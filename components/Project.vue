<template>
              <div class="card-container">
                <div v-for="c in count" :key="c" class="card">
                    <div class="card-image">
                        <img src="test.jpg" alt="" />
                    </div>
                    <div class="card-info">
                        <h2>A card name</h2>
                        <p>
                            Lorem ipsum dolor sit amet, consectetur adipiscing
                            elit.
                        </p>
                    </div>
                    <div class="card-icons">
                        <a href="#"> demo
                        </a>
                        <a href="#"> code
                        </a>
                    </div>
                    
                </div>
              </div>
</template>

<script>
export default {
  name: 'Project',
  props: {
    count: Number
  },
  
}
</script>

<style>
/* Add your styles here */
  .card-container {
    margin: 2rem;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    grid-template-rows: auto;
    gap: 2rem;
}

.card {
  font-family: 'Roboto', sans-serif;
    width: 100%;
    height: 30rem;
    border-radius: 5px;
    border: 1px solid #ddd;
    overflow: hidden;
    position: relative;
}

.card h2 {
  font-size: 1.5rem;
}

.card p {
  font-size: 1rem;
}

.card:hover {
    box-shadow: 0px 5px 10px rgba(0, 0, 0, 0.2);
}

.card-image {
    width: 100%;
    height: 60%;
    overflow: hidden;
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
    color: #444;
    font-size: 1.1rem;
}

.card-icons,
.card-lang {
    margin: 1rem;
    display: flex;
    align-items: center;
    gap: 1rem;
    color: #777;
    font-size: 0.9rem;
}

.card-lang {
    margin-top: 1rem;
}

@media screen and (max-width: 550px) {
    .card-container {
        grid-template-columns: 1fr;
        grid-template-rows: auto;
    }
}

</style>
