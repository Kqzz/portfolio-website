<script>
export default {
  data() {
    return {
      projects: [
        {
          id: 0,
          name: "MCsniperGO",
          dates: "2021 - present",
          description:
            "a free & open source Minecraft name sniper written in Go",
          links: [
            {
              id: 0,
              link: "https://github.com/Kqzz/MCsniperGO",
              img: "",
            },
          ],
        },
        {
          id: 1,
          name: "MCsniperPY",
          dates: "2020 - 2021",
          description:
            "a free & open source Minecraft name sniper written in Python",
        },
        {
          id: 2,
          name: "Atlas Sniper",
          dates: "2021 - Present",
          description:
            "closed source Minecraft name sniper focused on server scaling and Discord bot integration",
        },
      ],
    };
  },
};
</script>

<template>
  <div class="projects-wrapper">
    <div class="custom-shape-divider-top-1637614036">
      <svg
        data-name="Layer 1"
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 1200 120"
        preserveAspectRatio="none"
      >
        <path
          d="M321.39,56.44c58-10.79,114.16-30.13,172-41.86,82.39-16.72,168.19-17.73,250.45-.39C823.78,31,906.67,72,985.66,92.83c70.05,18.48,146.53,26.09,214.34,3V0H0V27.35A600.21,600.21,0,0,0,321.39,56.44Z"
          class="shape-fill"
        ></path>
      </svg>
    </div>
    <div class="projects">
      <h1 id="projects">Projects</h1>
      <div v-for="project in projects" v-bind:key="project.id">
        <div class="project">
          <h2>
            {{ project.name }}
          </h2>
          <div class="dates-line">
            <p class="dates">{{ project.dates }}</p>
            <div v-if="project.links != []">
              <!-- <a v-bind:href="link.link"> -->
              <!-- <img
                  v-bind:src="link.img"
                  alt="GitHub"
                  width="64"
                  height="64"
                  v-for="link in project.links"
                  v-bind:key="link.id"
                /> -->
              <!-- </a> -->
            </div>
          </div>
          <p class="description">{{ project.description }}</p>
        </div>
      </div>
    </div>
    <div class="custom-shape-divider-bottom-1637614252">
      <svg
        data-name="Layer 1"
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 1200 120"
        preserveAspectRatio="none"
      >
        <path
          d="M321.39,56.44c58-10.79,114.16-30.13,172-41.86,82.39-16.72,168.19-17.73,250.45-.39C823.78,31,906.67,72,985.66,92.83c70.05,18.48,146.53,26.09,214.34,3V0H0V27.35A600.21,600.21,0,0,0,321.39,56.44Z"
          class="shape-fill"
        ></path>
      </svg>
    </div>
  </div>
</template>

<style scoped>
.projects-wrapper {
  position: relative;
  background: #181618;
  padding: 0px;
  margin: 0px;
}

.projects {
  margin-right: 10%;
  color: white;
  padding-top: 10rem;
  padding-bottom: 7rem;
  margin-left: 10%;
  background-color: #181618;
  margin-bottom: 2rem;
}

h1 {
  font-size: 7rem;
  font-weight: bold;
  margin-bottom: 3rem;
}

.project h2,
.project .dates {
  font-size: 3.5rem;
  font-weight: bold;
  color: #181618;
  -webkit-text-stroke-width: 1px;
  -webkit-text-stroke-color: white;
  letter-spacing: 0.3rem;
  margin-bottom: 0.8rem;
}

.project .dates {
  font-size: 1.4rem;
  margin-bottom: 0.5rem;
}

.project .description {
  margin-bottom: 5rem;
  font-size: 1.5rem;
}

.dates-line {
  display: flex;
  align-items: center;
}

.custom-shape-divider-top-1637614036 {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  overflow: hidden;
  line-height: 0;
}

.custom-shape-divider-top-1637614036 svg {
  position: relative;
  display: block;
  width: calc(100% + 1.3px);
  height: 114px;
}

.custom-shape-divider-top-1637614036 .shape-fill {
  fill: #ffffff;
}

/** For mobile devices **/
@media (max-width: 767px) {
  .custom-shape-divider-top-1637614036 svg {
    width: calc(100% + 1.3px);
    height: 45px;
  }
}

.custom-shape-divider-bottom-1637614252 {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  overflow: hidden;
  line-height: 0;
  transform: rotate(180deg);
}

.custom-shape-divider-bottom-1637614252 svg {
  position: relative;
  display: block;
  width: calc(100% + 1.3px);
  height: 82px;
}

.custom-shape-divider-bottom-1637614252 .shape-fill {
  fill: #ffffff;
}

/** For mobile devices **/
@media (max-width: 767px) {
  .custom-shape-divider-bottom-1637614252 svg {
    width: calc(100% + 1.3px);
    height: 45px;
  }
}
</style>
