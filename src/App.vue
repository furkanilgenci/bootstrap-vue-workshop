<script>
export default {
  data() {
    return {
      projects: [
        { name: "Web page" },
        { name: "Backend project" },
        { name: "Marketing project" },
        { name: "Game project" },
        { name: "Our project" },
      ],
    };
  },
};
</script>

<template>
  <div>
    <div class="container-fluid bg-dark">
      <div class="row">
        <h1>Header</h1>
      </div>
    </div>
    <h2 class="page-title">Projects</h2>
    <div class="container">
      <div class="row">
        <div v-for="project in projects" :key="project.name" class="col-12 col-md-4 col-lg-3">
          <div class="card project-card">
            <div class="card-body">
              <h5 class="card-title">{{ project.name }}</h5>
              <p class="card-text">
                Some quick example text to build on the card title and make up
                the bulk of the card's content.
              </p>
              <a href="#" class="btn btn-primary">Go somewhere</a>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="container-fluid bg-warning page-footer">
      <div class="row">
        <h1>footer</h1>
      </div>
    </div>
  </div>
</template>

<style scoped>
.page-title {
  margin: 12px 8px;
}
.page-footer {
  margin-top: 24px;
}
.project-card {
  margin-top: 8px;
}
nav {
  width: 100%;
  font-size: 12px;
  margin-top: 2rem;
  position: absolute;
  top: 0;
  right: 0;
  display: flex;
  justify-content: flex-end;
  gap: 1rem;
  font-size: 1rem;
  padding: 1rem 0;
}
.logo {
  margin: 0 2rem 0 0;
}
.projects {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1rem;
}
</style>