<template>
  <div class="project">
    <h1>Our Projects</h1>
    <p>Take a look at some of our recent projects:</p>
    <div class="project-container">
      <div class="project-card" v-for="project in projects" :key="project.title">
        <img :src="project.image" :alt="project.title">
        <h2>{{ project.title }}</h2>
        <p>{{ project.description }}</p>
        <a :href="project.link" target="_blank">Learn More</a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ProjectView',
  data() {
    return {
      projects: [
        {
          title: 'Project 1',
          image: 'https://via.placeholder.com/300x200',
          description: 'This is a brief description of Project 1.',
          link: 'https://www.example.com/project1'
        },
        {
          title: 'Project 2',
          image: 'https://via.placeholder.com/300x200',
          description: 'This is a brief description of Project 2.',
          link: 'https://www.example.com/project2'
        },
        {
          title: 'Project 3',
          image: 'https://via.placeholder.com/300x200',
          description: 'This is a brief description of Project 3.',
          link: 'https://www.example.com/project3'
        }
      ]
    }
  }
}
</script>

<style scoped>
.project {
  text-align: center;
  padding: 20px;
}

.project-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}

.project-card {
  margin: 20px;
  padding: 20px;
  border: 1px solid #ccc;
  border-radius: 10px;
  width: 30%;
}

.project-card img {
  width: 100%;
  height: 150px;
  object-fit: cover;
  border-radius: 10px 10px 0 0;
}

.project-card h2 {
  margin-top: 0;
}

.project-card a {
  text-decoration: none;
  color: #337ab7;
}

.project-card a:hover {
  color: #23527c;
}
</style>