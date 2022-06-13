<template>
  <main class="dark main">
    <aside class="indicator">Indicator</aside>
  <article class="">
    <Header/>
  <section class="sect sect--hero">
    <div class="">
      <p class="">Gbalam Prince</p>
    <h1 class="">Full Stack Developer</h1>
    </div>
    <div class="bubbles">
      <div class="">G</div>
      <div class="">G</div>
      <div class="">L</div>
    </div>
  </section>
  <section class="sect sect--projects">
    <h2 class="">Selected Projects</h2>
    <div class="projects">
      <div class="project">
        <div class="project__image">
          <!-- <img src="../static/showcase.webp" alt=""> -->
        </div>
        <div class="project__details">
          <div class="">
            <h3 class="">Project 1</h3>
        <p>Description</p>
          </div>
          <a class="project__button" href="/">B</a>
        </div>
      </div>
      <div class="project">
        <div class="project__image">
          <!-- <img src="../static/showcase.webp" alt=""> -->
        </div>
        <div class="project__details">
          <div class="">
            <h3 class="">Project 1</h3>
        <p>Description</p>
          </div>
          <a class="project__button" href="/">B</a>
        </div>
      </div>
    </div>
  </section>
  <section class="sect sect--about">
    <p class="">I have a passion for creating user experiences that are seamless, meaningful and impactful.</p>
    <h2>About me</h2>
    <div class="">
      a
    </div>
  </section>
  <section class="sect sect--experience">
    <h2 class="">Work Experience</h2>
    <WorkExperience/>
  </section>
  <section class="sect sect--more-works">
    <h2 class="">More Works</h2>
    <MoreWorks />
  </section>
  <section class="sect sect--contact">
    <h2>Let's work together</h2>
    <p>asdmao</p>
    <a>Write an Email</a>
    <form action="">
      
    </form>
  </section>
  <footer>
    Designed and developed by Prince Codes
    Version 2022
  </footer>
    </article>
    <aside class="">
      Links
    </aside>
  </main>
</template>

<script>
export default {
    name: "IndexPage",
    data() {
        return {
            message: 0
        };
    },
}
</script>