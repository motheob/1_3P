<template>
  <div class="projects-view">
    <h1>Projects</h1>
    <div class="project-cards">
      <div class="project-card">
        <h2>1.1P</h2>
        <p>HTML and CSS web page incorporating elements such as image, table, form etc.</p>
        <a href="http://github.com/motheob/1_1P" target="_blank">GitHub repo</a>
      </div>

      <div class="project-card">
        <h2>1.2P</h2>
        <p>Implementing Responsive Web Design principles to create a web page using HTML and CSS.</p>
        <a href="http://github.com/motheob/1_2P" target="_blank">GitHub repo</a>
      </div>
    </div>
  </div>
</template>

<style scoped>
.projects-view {
  text-align: center;
}

.project-cards {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
}

.project-card {
  width: 300px;
  padding: 20px;
  margin: 20px;
  border: 1px solid #ccc;
  border-radius: 5px;
  text-align: left;
}

.project-card h2 {
  font-size: 1.5rem;
}

.project-card a {
  text-decoration: none;
}
</style>