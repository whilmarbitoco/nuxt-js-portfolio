<template>
  <li>
    <span>{{ skill }}</span>
    <div class="progress-bar">
      <div class="progress" :style="{ width: progress }"></div>
    </div>
  </li>
</template>

<script>
export default {
  name: 'Skill-Item',
  props: {
    skill: String,
    progress: String
  }
}
</script>

<style>
/* Add your styles here */
ul {
    list-style-type: none;
    padding: 0;
}

li {
    margin-bottom: 0.5rem;
}

.interest ul {
    padding: 1rem;
}

.fa {
    color: #56b4c9;
    font-size: 1.5rem;
    margin-right: 0.5rem;
}

span {
    display: inline-block;
    width: 100px;
    font-weight: bold;
}

.progress-bar {
    height: 10px;
    background-color: #f5f5f5;
    border-radius: 10px;
    overflow: hidden;
}

.progress {
    height: 100%;
    background-color: #56b4c9;
}

</style>
