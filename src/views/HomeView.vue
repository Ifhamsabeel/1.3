<template>
  <div class="about">
    <h1>About Me</h1>
    <p>
      I'm a passionate web developer with a love for creating beautiful and functional websites. I
      specialize in front-end development and have a strong foundation in HTML, CSS, and JavaScript.
      My goal is to build user-friendly and visually appealing web experiences that leave a lasting
      impression.
    </p>
    <p>
      I am currently a fresher at Deakin University studying my Bachelors. I have a keen interest in
      web development and I am always looking to learn new things and apply them to my projects.
    </p>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
  }

  .about h1 {
    font-size: 2.5rem;
  }

  .about p {
    font-size: 1.2rem;
    max-width: 600px;
    margin: 20px 0;
  }
}

@media (max-width: 1023px) {
  .about {
    padding: 20px;
    text-align: left;
  }

  .about h1 {
    font-size: 2rem;
  }

  .about p {
    font-size: 1rem;
    max-width: 100%;
    margin: 15px 0;
  }
}
</style>
