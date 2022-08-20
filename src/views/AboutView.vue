<template>
    <nav class="navbar navbar-dark navbar-expand-lg fixed-top bg-dark portfolio-navbar">
      <div class="container">
        <!-- <a class="navbar-brand" href="#">HikariKage</a> -->
        <img style="width: 50px;height: 50px;" src="../assets/rocket-icon.png">
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
    
    <main class="page lanidng-page">
      <section class="portfolio-block block-intro" style="background-repeat: round; background-color: rgba(65,129,156,0);">
          <div class="container">
              <!-- :style="{ 'background-image' : `url(${require(profileImage)})`}" -->
                <!-- <img src="../assets/profile2.png"> -->
              <div class="avatar" id="targetProfile"></div>
              <div class="about-me">
                  <p>Hello! I am <span class="fw-bold">Marckus Balingit</span>.&nbsp;</p>
              </div>
          </div>
      </section>
      <section class="portfolio-block photography">
          <div class="container">
              <div class="row no-gutters">
                  <div class="col-md-6 col-lg-4 item zoom-on-hover"><a href="#"><img class="img-fluid image" src="../assets/nature/image5.jpg"></a></div>
                  <div class="col-md-6 col-lg-4 item zoom-on-hover"><a href="#"><img class="img-fluid image" src="../assets/nature/image2.jpg"></a></div>
                  <div class="col-md-6 col-lg-4 item zoom-on-hover"><a href="#"><img class="img-fluid image" src="../assets/tech/image4.jpg"></a></div>
              </div>
          </div>
      </section>
      <section class="portfolio-block call-to-action border-bottom"></section>
    </main>

    <section class="portfolio-block website">
      <div class="container">
          <div class="row align-items-center">
              <div class="col-md-12 col-lg-5 offset-lg-1 text">
                  <h3>Website Project</h3>
                  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean eget velit ultricies, feugiat est sed, efr nunc, vivamus vel accumsan dui. Quisque ac dolor cursus, volutpat nisl vel, porttitor eros.</p>
              </div>
          </div>
      </div>
  </section>
  <footer class="page-footer">
    <div class="container">
        <div class="links"><a href="#">About me</a><a href="#">Contact me</a><a href="#">Projects</a></div>
        <div class="social-icons">
          <a href="#"><i class="fa fa-facebook-f"></i></a>
          <a href="#"><i class="fa fa-instagram"></i></a>
          <a href="#"><i class="fa fa-twitter"></i></a>
        </div>
    </div>
</footer>

</template>

<script>
import { defineComponent } from 'vue'

export default defineComponent({
  setup() {
    let profileImage = "@/src/assets/profile2.png"
    
    return {
      profileImage
    }
  },
})
</script>


<style scoped>
.portfolio-navbar {
  padding-top: 1.2rem;
  padding-bottom: 1.2rem;
}

.bg-dark {
  background-color: #343A40 !important;
}

.nav-item {
  padding-right: 2rem !important;
}

#targetProfile {
  background-image: url('~@/assets/profile2.png');
}

.portfolio-block {
    padding-bottom: 60px;
    padding-top: 60px
}

.portfolio-block .heading {
    margin-bottom: 50px;
    text-align: center
}

.portfolio-block .heading h2 {
    font-weight: 700;
    font-size: 1.4rem;
    text-transform: uppercase
}

.portfolio-block .heading p {
    text-align: center;
    max-width: 420px;
    margin: auto;
    opacity: .7
}

.portfolio-block.block-intro {
    text-align: center
}

.portfolio-block.block-intro .about-me {
    max-width: 800px;
    margin: 0 auto
}

.portfolio-block.block-intro p {
    font-size: 1.5em;
    font-weight: 300;
    margin-bottom: 30px
}

.portfolio-block.block-intro .avatar {
    width: 150px;
    height: 150px;
    background-size: cover;
    background-repeat: no-repeat;
    margin: auto;
    border-radius: 100px;
    margin-bottom: 30px
}

.portfolio-block.photography {
    padding-top: 0;
    padding-bottom: 0
}

.portfolio-block.photography .item a img {
    transition: .8s ease
}

.portfolio-navbar.fixed-top+.page {
    padding-top: 100px;
}

.page-footer {
    padding-top: 35px;
    border-top: 1px solid #ddd;
    text-align: center;
    padding-bottom: 20px
}

.page-footer a {
    margin: 0 10px;
    color: #282b2d;
    font-size: 18px;
    text-decoration: none;
}

.page-footer .links,.page-footer a {
    display: inline-block
}

.page-footer .social-icons {
    margin-top: 20px;
    margin-bottom: 16px
}

.page-footer .social-icons a {
    font-size: 18px;
    margin: 0 3px;
    color: #fff;
    border: 1px solid;
    opacity: .75;
    border-radius: 50%;
    width: 36px;
    display: inline-block;
    height: 36px;
    text-align: center;
    background-color: #c5c9d2;
    line-height: 34px
}

.page-footer .social-icons a:hover {
    opacity: 1
}


/* @media (min-width: 576px) {
    .navbar {
        padding-top:1.2rem;
        padding-bottom: 1.2rem
    }

    .portfolio-navbar.fixed-top+.page {
        padding-top: 5.5rem;
    }
} */
</style>
