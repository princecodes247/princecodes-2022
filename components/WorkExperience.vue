
<template>
  <div class="experience__list">
    <div class="experience_companies">
      <div :class="{ active: selectedJob === job }" class="experience_company" @click="changeSelectedJob" v-for="job in Object.keys(jobs)">
        {{ job }}
      </div>
    </div>
      <div class="experience__description" >
        <h4>
            {{ jobs[selectedJob].title }}
            @{{ selectedJob }}
        </h4>
        <h5>
            {{ jobs[selectedJob].date }}
        </h5>
        <div class="">
            <p v-for="point in jobs[selectedJob].points">
        {{ point }}
        </p>
        </div>
      </div>
  </div>
</template>
<style>
</style>


<script>
export default {
  name: "WorkExperience",
  methods: {
  changeSelectedJob(event) {
    this.selectedJob = event.target.innerText;
  }
  },
  data() {
    return {
        selectedJob: "AstroSoft",
      jobs: {
          
        "AstroSoft": {
          title: "Full Stack Developer",
          date: "2020 - Present",
          points: [
            "Developed and maintained code for in-house and client websites primarily using HTML, CSS, Sass, JavaScript, and jQuery",
            "Manually tested sites in various browsers and mobile devices to ensure cross-browser compatibility and responsiveness",
            "Clients included JetBlue, Lovesac, U.S. Cellular, U.S. Department of Defense, and more",
          ],
        },
          "AyaweiSoft":{
          title: "Full Stack Developer",
          date: "2019 - 2020",
          points: [
            "Developed and maintained code for in-house and client websites primarily using HTML, CSS, Sass, JavaScript, and jQuery",
            "Manually tested sites in various browsers and mobile devices to ensure cross-browser compatibility and responsiveness",
            "Clients included JetBlue, Lovesac, U.S. Cellular, U.S. Department of Defense, and more",
          ],
        },
          "Eddify": {
          title: "Full Stack Developer",
          date: "2018 - 2019",
          points: [
            "Developed and maintained code for in-house and client websites primarily using HTML, CSS, Sass, JavaScript, and jQuery",
            "Manually tested sites in various browsers and mobile devices to ensure cross-browser compatibility and responsiveness",
            "Clients included JetBlue, Lovesac, U.S. Cellular, U.S. Department of Defense, and more",
          ],
        },
          "Uneleap.inc": {
          title: "Full Stack Developer",
          date: "2017 - 2018",
          points: [
            "Developed and maintained code for in-house and client websites primarily using HTML, CSS, Sass, JavaScript, and jQuery",
            "Manually tested sites in various browsers and mobile devices to ensure cross-browser compatibility and responsiveness",
            "Clients included JetBlue, Lovesac, U.S. Cellular, U.S. Department of Defense, and more",
          ],
        },
          "Trident.inc": {
          title: "Full Stack Developer",
          date: "2016 - 2017",
          points: [
            "Developed and maintained code for in-house and client websites primarily using HTML, CSS, Sass, JavaScript, and jQuery",
            "Manually tested sites in various browsers and mobile devices to ensure cross-browser compatibility and responsiveness",
            "Clients included JetBlue, Lovesac, U.S. Cellular, U.S. Department of Defense, and more",
          ],
        },
          "3reen": {
          title: "Full Stack Developer",
          date: "2015 - 2016",
          points: [
            "Developed and maintained code for in-house and client websites primarily using HTML, CSS, Sass, JavaScript, and jQuery",
            "Manually tested sites in various browsers and mobile devices to ensure cross-browser compatibility and responsiveness",
            "Clients included JetBlue, Lovesac, U.S. Cellular, U.S. Department of Defense, and more",
          ],
        },
      
      },
    };
  },
};
</script>
