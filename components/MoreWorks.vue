
<template>
  <div :[attributeName]="url" class="more_works">
    <div class="more_works__item" v-for="work in works">
      <div class="more_works__item__title">
        <h5>{{ work.title }}</h5>
      </div>
      <div class="more_works__item__date">
        <!-- <p>{{ work.date }}</p> -->
      </div>
      <!-- <div class="more_works__item__points">
                <ul>
                    <li v-for="point in jobs[selectedJob].points">
                        <p>{{point}}</p>
                    </li>
                </ul>
            </div> -->
    </div>
  </div>
</template>

<script>
export default {
  name: "MoreWorks",
  methods: {
    showCover(event) {
      // this.selectedJob = event.target.innerText;
    },
  },
  data() {
    return {
      works: [
        {
          title: "CloudPay",
          date: "2001",
          points: [
            "Developed and maintained code for in-house and client websites primarily using HTML, CSS, Sass, JavaScript, and jQuery",
            "Manually tested sites in various browsers and mobile devices to ensure cross-browser compatibility and responsiveness",
            "Clients included JetBlue, Lovesac, U.S. Cellular, U.S. Department of Defense, and more",
          ],
        },
        {
          title: "Cardde",
          date: "2019 - 2020",
          points: [
            "Developed and maintained code for in-house and client websites primarily using HTML, CSS, Sass, JavaScript, and jQuery",
            "Manually tested sites in various browsers and mobile devices to ensure cross-browser compatibility and responsiveness",
            "Clients included JetBlue, Lovesac, U.S. Cellular, U.S. Department of Defense, and more",
          ],
        },
        {
          title: "InstaNovella",
          date: "2018 - 2019",
          points: [
            "Developed and maintained code for in-house and client websites primarily using HTML, CSS, Sass, JavaScript, and jQuery",
            "Manually tested sites in various browsers and mobile devices to ensure cross-browser compatibility and responsiveness",
            "Clients included JetBlue, Lovesac, U.S. Cellular, U.S. Department of Defense, and more",
          ],
        },
      ],
    };
  },
};
</script>

