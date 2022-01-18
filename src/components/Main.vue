<script>
export default {};
</script>

<template>
  <div class="content">
    <div>
      <h1>
        Hey, I'm<br />
        <span style="color: #b363cc"> Kqzz</span>
      </h1>
      <p class="subhead">
        I'm a <span style="color: #b363cc">software developer</span> working
        with Go & Python
      </p>
      <div class="content-btns">
        <a class="projects btn" href="#projects">Projects</a>
        <a class="contact btn" href="#contact">Contact</a>
      </div>
    </div>
    <div class="image"></div>
  </div>
</template>

<style scoped>
.content h1 {
  font-size: 10vw;
  font-weight: bold;
  margin-bottom: 35px;
  margin-top: 24px;
}

.content-btns {
  /* We first create a flex layout context */
  display: flex;

  /* Then we define the flow direction
     and if we allow the items to wrap
   * Remember this is the same as:
   * flex-direction: row;
   * flex-wrap: wrap;
   */
  flex-flow: row wrap;

  justify-content: left;
}

/* Medium screens */
@media all and (max-width: 970px) {
  .content-btns {
    /* When on medium sized screens, we center it by evenly distributing empty space around items */
    flex-direction: column;
  }
}

@media all and (max-width: 565px) {
  .image {
    visibility: hidden;
  }
}

.btn {
  margin-bottom: 1rem;
}

p {
  font-size: 1rem;
}

.content {
  margin-top: 5%;
  text-align: left;
  display: flex;
  justify-content: space-between;
  margin-right: 10%;
  margin-left: 10%;
  margin-bottom: 20rem;
}

.subhead {
  font-size: 1.3rem;
  margin-bottom: 2em;
}

.image {
  max-width: 32rem;
  width: 100%;
  height: 600px;
  background: url("../assets/hero-image.gif");
  background-repeat: no-repeat;
  background-size: 300%;
  background-position-x: -130px;
  filter: drop-shadow(4px 4px 7px rgba(0, 0, 0, 0.4));
  border-radius: 100px 0px 22px;
}

.image div {
  background-color: #181618;
}

.btn.projects {
  border: none;
  -webkit-appearance: none;
  color: white;

  background: -webkit-gradient(to right, #ca85c1 0%, #79408b 50%, #f195b1 100%);
  background: linear-gradient(to right, #ca85c1 0%, #79408b 50%, #f195b1 100%);
  background-size: 500%;
  box-shadow: 0 0.5rem 1rem rgba(0, 0, 0, 0.35);
}

.btn:hover {
  cursor: pointer;
}

.btn.projects:hover {
  animation-name: gradient;
  -webkit-animation-name: gradient;
  animation-duration: 2s;
  -webkit-animation-duration: s;
  animation-iteration-count: 1;
  -webkit-animation-iteration-count: 1;
  animation-fill-mode: forwards;
  -webkit-animation-fill-mode: forwards;
}

@keyframes gradient {
  0% {
    background-position: 0% 50%;
  }
  100% {
    background-position: 100%;
  }
}
</style>
