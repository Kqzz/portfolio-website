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
      <a class="projects btn" href="#projects">Projects</a>
      <a class="contact btn" href="#contact">Contact</a>
    </div>
    <div>
      <div class="image"></div>
    </div>
  </div>
</template>

<style scoped>
.content h1 {
  font-size: 7rem;
  font-weight: bold;
  margin-bottom: 35px;
  margin-top: 24px;
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
  margin-bottom: 10rem;
}

.subhead {
  font-size: 1.3rem;
  margin-bottom: 2em;
}

.image {
  width: 32rem;
  height: 40rem;
  background: url("../assets/hero-image.gif");
  background-repeat: no-repeat;
  background-size: 200%;
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
