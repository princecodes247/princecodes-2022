<template>
  <main class="dark main">
    <aside class="indicator">Indi</aside>
    <article class="">
      <Header />
      <section class="sect sect--hero">
        <div class="bubbles">
          <div class="sect--hero__bubble">G</div>
          <div class="sect--hero__bubble">G</div>
          <div class="sect--hero__bubble">L</div>
        </div>
        <div class="">
          <p class="">Gbalam Prince</p>
          <h1 class="">Full Stack Developer</h1>
        </div>
        <div class="scroll_indicator">Scroll down</div>
      </section>
      <!-- <MouseTracker v-slot="{ x, y }">
        Mouse is at: {{ x }}, {{ y }}
      </MouseTracker> -->
      <section class="sect sect--projects">
        <h2 class="">Selected Projects</h2>
        <div class="projects">
          <div class="project" v-for="project in projects">
            <div class="project__image">
              <!-- <img src="../static/showcase.webp" alt=""> -->
            </div>
            <div class="project__details">
              <div class="">
                <h3 class="">{{ project.name }}</h3>
                <p>{{ project.desc }}</p>
              </div>
              <a class="project__button" href="/">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                  stroke-width="2"
                >
                  <path
                    stroke-linecap="round"
                    stroke-linejoin="round"
                    d="M17 8l4 4m0 0l-4 4m4-4H3"
                  />
                </svg>
              </a>
            </div>
          </div>
        </div>
      </section>
      <section class="sect sect--about">
        <p class="sect--about__details">
          I have a passion for creating user experiences that are seamless,
          meaningful and impactful.
        </p>
        <h2>About me</h2>
        <div class="">a</div>
      </section>
      <section class="sect sect--experience">
        <h2 class="">Work Experience</h2>
        <WorkExperience />
      </section>
      <section class="sect sect--more-works">
        <h2 class="">More Works</h2>
        <MoreWorks />
      </section>
      <section class="sect sect--contact">
        <h2>Let's work together</h2>
        <div class="sect--contact__options">
          <div class="sect--contact__links">
            <a href="https://www.github.com/princecodes247">Github</a>
            <a href="https://www.linkedin.com/in/gbalamprince">LinkedIn</a>
            <a href="https://www.twitter.com/gbalamprince">Twitter</a>
            <a href="https://www.hashnode.com/gbalamprince">Hashnode</a>
          </div>
          <a href="mailto:princecodes247@gmail.com">Write an Email</a>
        </div>
        <form action=""></form>
      </section>
      <footer>Designed and developed by Prince Codes Version 2022</footer>
    </article>
    <aside class="">Links</aside>
    <div class="main_background">
      <div class="main_background__shape"></div>
    </div>
  </main>
</template>

<script>
export default {
  name: "IndexPage",
  data() {
    return {
      projects: [
        {
          name: "Veldora",
          desc: "A showcase of my work",
        },
        {
          name: "FirstTime2020",
          desc: "A showcase of my work",
        },
      ],
    };
  },
};
</script>