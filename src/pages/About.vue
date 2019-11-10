<template>
  <Layout>
    <div class="about-page">
      <div class="content-container">
        <h1 class="content-heading">Hi! I am Shubham Zanwar</h1>
        <div class="content">
        <div class="content-block"></div>
          <p>I am a full stack software developer working in an agile 
          environment. I have professional expertise in building 
          scalable web and mobile applications. I am currently living 
          and working from Bangalore, India. I am passionate about 
          code quality, performance and have a knack for refactoring!</p>
          <p>I primarily work with Javascript - I love react, vue and 
            absolutely enjoy exploring JS quirks. In my free time, I also 
            hack around with Python and Golang. You can find some of 
            my work here. I also document things that interest me on 
            my blog on medium. You should totally check it out!</p>
          <p>Outside work, I like listening to music - I am an avid Beatles 
            fan. I also watch football (Chelsea FC, FTW), stand up 
            comedy shows and sometimes learn card magic on 
            YouTube. I am also fairly active on Twitter and Instagram.</p>
        </div>
      </div>
      <div class="image-container">
        <g-image src="~/assets/profile-picture.jpg" class="profile-picture"/>
        <div class="skills">
          <font-awesome :icon="['fas', 'code']" class="skill-icon" />
          HTML, CSS, JS, React native, ReactJS
          VueJS, nodeJS, Python, GoLang
        </div>
        <div class="skills">
          <font-awesome :icon="['fas', 'tools']" class="skill-icon" />
          Git, Docker, Kubernetes, Terraform, 
          Microservices, CircleCI
        </div>
        <div class="skills">
          <font-awesome :icon="['fas', 'briefcase']" class="skill-icon" />
          Agile, TDD, Digital consulting
        </div>
      </div>
    </div>
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'About'
  }
}
</script>

<style scoped>
  .about-page {
    flex: 1;
    display: flex;
    flex-direction: row;
    padding: 0 3rem 1rem;
  }

  .content-container {
    flex: 2;
    /* border: 1px solid black; */
    margin-right: 2rem;
  }

  .content-heading {
    font-size: 3rem;
    font-weight: 400;
  }

  .content {
    width: 82%;
    font-weight: 400;
    font-size: 1.25rem;
    position: relative;
  }

  .content-block {
    position: absolute;
    background: #B0F3D7;
    z-index: -1;
    height: 130%;
    width: 100%;
    bottom: -10%;
    right: -20%;
  }

  .image-container {
    flex: 1;
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top: 2.67rem;
  }

  .profile-picture {
    width: 18rem;
  }

  .skills {
    width: 20rem;
    font-weight: bold;
    margin-top: 1.25rem;
    color: #AAAAAA;
    display: flex;
    align-items: center;
  }

  .skill-icon {
    margin-right: 1rem;
    color: #999;
  }

  @media only screen and (max-width: 768px) {
    .about-page{
      display: -webkit-box;
      -webkit-box-orient: vertical;
      -moz-box-orient: vertical;
      box-orient: vertical;
      -webkit-box-direction: reverse;
      -moz-box-direction: reverse;
      box-direction: reverse;
      padding: 0 0 1rem;
    }
    .content-container {
      margin-right: 0;
      margin-top: 2rem;
    }
    .content-heading {
      font-size: 1.2rem;
    }
    .content-block {
      width: 100%;
      height: 100%;
      bottom: 0;
      right: 0;
    }
    .content {
      font-size: 0.75rem;
      width: 100%;
    }
    .skills {
      font-size: 0.5rem;
      width: 18rem;
    }
  }

</style>
