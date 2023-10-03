<template>
  <div class="project-card">
    <h2>{{ title }}</h2>
    <p>{{ description }}</p>
    <a :href="detailsLink">View Details</a>
  </div>
</template>

<script>
export default {
  props: {
    title: String,
    description: String,
    detailsLink: String
  }
}
</script>

<style scoped>
.project-card {
  width: calc(50% - 20px);
  background-color: #6b6a6a;
  padding: 20px;
  border-radius: 5px;
  text-align: center;
  margin-bottom: 20px;
  box-sizing: border-box;
  margin-top: 10px;
}

.project-card h2 {
  font-size: 1.5rem;
}

.project-card p {
  margin-top: 10px;
  font-size: 1rem;
}

.project-card a {
  display: block;
  margin-top: 10px;
  text-decoration: none;
  font-weight: bold;
  color: #00bd7e;
}

@media (max-width: 1023px) {
  .project-card {
    width: 100%;
    padding: 10px;
  }
}
</style>
