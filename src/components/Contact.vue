<script>
export default {};
</script>

<template>
  <div id="contact">
    <h1>Contact</h1>
    <p>mail: kqzz [at] kqzz [dot] me</p>
    <div class="contact-btns">
      <a href="https://discordid.netlify.app/?id=703244711187578911" class="btn"
        >discord</a
      >
      <a href="https://github.com/Kqzz" class="btn">github</a>
      <a href="https://keybase.io/kqzz" class="btn">keybase</a>
    </div>
  </div>
</template>

<style scoped>
#contact {
  margin-right: 10%;
  margin-left: 10%;
}

.contact-btns {
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

.btn {
  margin-bottom: 1rem;
}

/* Medium screens */
@media all and (max-width: 970px) {
  .contact-btns {
    /* When on medium sized screens, we center it by evenly distributing empty space around items */
    flex-direction: column;
  }
}

h1 {
  font-size: 500%;
  font-weight: bold;
  margin-bottom: 3rem;
  background: linear-gradient(to right, #ca85c1 0%, #79408b 50%, #f195b1 100%);
  -webkit-text-fill-color: transparent;
  -webkit-background-clip: text;
  background-clip: text;
  overflow: visible;
}

p {
  font-size: 1.5rem;
  margin-bottom: 3rem;
}
</style>
