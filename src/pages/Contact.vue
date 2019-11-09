<template>
  <Layout>
    <div class="contact-page">
        <h1 class="contact-heading">You can reach out to me through email</h1>
        <a href="mailto:zanwar.shubham@gmail.com" class="contact-links medium-text">zanwar.shubham@gmail.com</a>
        <h3 class="contact-sub-heading">I am also available on <a href="" class="contact-links">Twitter</a> and <a href="" class="contact-links">instagram</a></h3>
    </div>
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'Contact'
  }
}
</script>

<style scoped>
  .contact-page {
    flex: 1;
    text-align: center;
    padding-top: 2rem;
  }

  .medium-text {
    font-size: 3rem;
  }

  .contact-heading {
    font-size: 3.5rem;
    margin: 1rem 0;
  }

  .contact-links {
    text-decoration: none;
    color: #4DCA95;
    font-weight: bold;
  }

  .contact-sub-heading {
    font-size: 2rem;
    margin: 1rem 0;
  }

  @media only screen and (max-width: 768px) {
    .contact-heading {
      font-size: 2rem;
    }
    .contact-sub-heading {
      font-size: 1.25rem;
    }

    .medium-text {
        font-size: 1.5rem;
    }
  }
</style>
