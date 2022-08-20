<template>
    <nav class="navbar navbar-dark navbar-expand-lg fixed-top bg-dark portfolio-navbar">
      <div class="container">
        <!-- <a class="navbar-brand" href="#">HikariKage</a> -->
        <img style="width: 50px;height: 50px;" src="../../assets/rocket-icon.png">
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="nav navbar-nav ms-auto fw-bold">
            <li class="nav-item"><a class="nav-link active" aria-current="page" href="#">Home</a></li>
            <li class="nav-item"><a class="nav-link" href="#">Projects</a></li>
            <li class="nav-item"><a class="nav-link" href="#">Mini Projects</a></li>
            <li class="nav-item"><a class="nav-link">Email</a></li>
          </ul>
        </div>
      </div>
    </nav>
</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
    name: 'navbar',
    setup() {
        
    },
})
</script>
