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
          <p class="hero__name">Gbalam Prince</p>
          <h1 class="hero__title">
            Full Stack <span class="highlight">Developer</span>
          </h1>
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
              <img
                :src="
                  require(`../assets/projects/${project.name.toLowerCase()}.png`)
                "
                :alt="project.name"
              />
            </div>
            <div class="project__details">
              <div class="project__text">
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
      <section class="sect sect--about" id="about">
        <p class="sect--about__details">
          I have a passion for creating user experiences that are seamless,
          meaningful and impactful.
        </p>
        <h2>About me</h2>
        <a href="#contact" class="bubble_link">Say hi</a>
      </section>
      <section class="sect sect--experience">
        <h2 class="">Work Experience</h2>
        <WorkExperience />
      </section>
      <section class="sect sect--more-works">
        <h2 class="">More Works</h2>
        <MoreWorks />
      </section>
      <section class="sect sect--contact" id="contact">
        <h2>Let's work together</h2>
        <div class="sect--contact__options">
          <div class="sect--contact__links">
            <a href="https://www.github.com/princecodes247">
              <svg
                width="24"
                height="24"
                role="img"
                viewBox="0 0 24 24"
                fill="currentColor"
                xmlns="http://www.w3.org/2000/svg"
              >
                <title>GitHub icon</title>
                <path
                  d="M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.205 11.385.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61C4.422 18.07 3.633 17.7 3.633 17.7c-1.087-.744.084-.729.084-.729 1.205.084 1.838 1.236 1.838 1.236 1.07 1.835 2.809 1.305 3.495.998.108-.776.417-1.305.76-1.605-2.665-.3-5.466-1.332-5.466-5.93 0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 0 0 1.005-.322 3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 2.28-1.552 3.285-1.23 3.285-1.23.645 1.653.24 2.873.12 3.176.765.84 1.23 1.91 1.23 3.22 0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 2.22 0 1.606-.015 2.896-.015 3.286 0 .315.21.69.825.57C20.565 22.092 24 17.592 24 12.297c0-6.627-5.373-12-12-12"
                ></path>
              </svg>
              <p>Github</p>
            </a>
            <a href="https://www.linkedin.com/in/gbalamprince">
              <svg
                width="24"
                height="24"
                role="img"
                viewBox="0 0 24 24"
                fill="currentColor"
                xmlns="http://www.w3.org/2000/svg"
              >
                <title>LinkedIn icon</title>
                <path
                  d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433c-1.144 0-2.063-.926-2.063-2.065 0-1.138.92-2.063 2.063-2.063 1.14 0 2.064.925 2.064 2.063 0 1.139-.925 2.065-2.064 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"
                ></path>
              </svg>
              <p>LinkedIn</p>
            </a>
            <a href="https://www.twitter.com/gbalamprince">
              <svg
                width="24"
                height="24"
                role="img"
                viewBox="0 0 24 24"
                fill="currentColor"
                xmlns="http://www.w3.org/2000/svg"
              >
                <title>Twitter icon</title>
                <path
                  d="M23.954 4.569c-.885.389-1.83.654-2.825.775 1.014-.611 1.794-1.574 2.163-2.723-.951.555-2.005.959-3.127 1.184-.896-.959-2.173-1.559-3.591-1.559-2.717 0-4.92 2.203-4.92 4.917 0 .39.045.765.127 1.124C7.691 8.094 4.066 6.13 1.64 3.161c-.427.722-.666 1.561-.666 2.475 0 1.71.87 3.213 2.188 4.096-.807-.026-1.566-.248-2.228-.616v.061c0 2.385 1.693 4.374 3.946 4.827-.413.111-.849.171-1.296.171-.314 0-.615-.03-.916-.086.631 1.953 2.445 3.377 4.604 3.417-1.68 1.319-3.809 2.105-6.102 2.105-.39 0-.779-.023-1.17-.067 2.189 1.394 4.768 2.209 7.557 2.209 9.054 0 13.999-7.496 13.999-13.986 0-.209 0-.42-.015-.63.961-.689 1.8-1.56 2.46-2.548l-.047-.02z"
                ></path>
              </svg>
              <p>Twitter</p>
            </a>
            <a href="https://www.hashnode.com/gbalamprince">
              <svg
                width="24"
                height="24"
                xmlns="http://www.w3.org/2000/svg"
                fill="none"
                viewBox="0 0 24 24"
                stroke="currentColor"
              >
                <path
                  stroke-linecap="round"
                  stroke-linejoin="round"
                  stroke-width="2"
                  d="M3.055 11H5a2 2 0 012 2v1a2 2 0 002 2 2 2 0 012 2v2.945M8 3.935V5.5A2.5 2.5 0 0010.5 8h.5a2 2 0 012 2 2 2 0 104 0 2 2 0 012-2h1.064M15 20.488V18a2 2 0 012-2h3.064M21 12a9 9 0 11-18 0 9 9 0 0118 0z"
                ></path>
              </svg>
              <p>Hashnode</p>
            </a>
            <a
              href="https://api.whatsapp.com/send?phone=2349011308292&text=Hi!!!%20I%27m"
            >
              <svg
                width="24"
                height="24"
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 24 24"
                fill="currentColor"
              >
                <path d="M0 0h24v24H0z" fill="none"></path>
                <path
                  d="M20.01 15.38c-1.23 0-2.42-.2-3.53-.56a.977.977 0 00-1.01.24l-1.57 1.97c-2.83-1.35-5.48-3.9-6.89-6.83l1.95-1.66c.27-.28.35-.67.24-1.02-.37-1.11-.56-2.3-.56-3.53 0-.54-.45-.99-.99-.99H4.19C3.65 3 3 3.24 3 3.99 3 13.28 10.73 21 20.01 21c.71 0 .99-.63.99-1.18v-3.45c0-.54-.45-.99-.99-.99z"
                ></path>
              </svg>
              <p>WhatsApp</p></a
            >
          </div>
          <a href="mailto:princecodes247@gmail.com">Write an Email</a>
        </div>
        <form action=""></form>
      </section>
      <footer>Designed and developed by Prince Codes Version 2022</footer>
    </article>
    <aside class="">Lin</aside>
    <div class="main_background">
      <div class="main_background__shape"></div>
    </div>
  </main>
</template>

<script>
export default {
  name: "IndexPage",
  //   computed: {
  //   projectImage () {
  //     if (!this.selectedDog) {
  //       return
  //     }

  //     const fileName = this.selectedDog.toLowerCase()

  //     return require(`../assets/doggos/${fileName}.jpg`) // the module request
  //   }
  // },
  data() {
    return {
      projects: [
        {
          name: "Veldora",
          desc: "A PaaS (Platform as a Service) for managing your form and email data.",
        },
        {
          name: "Glassmorphism Generator",
          desc: "A dev tool for generating glassmorphism shapes.",
        },
      ],
    };
  },
};
</script>