<template>
  <Layout>
    
    <!-- Learn how to use images here: https://gridsome.org/docs/images -->
    <g-image class="profile" alt="Profile" src="~/assets/profile.jpg" width="130" />
    
    <h1 class="title">Tommy Vedvik 🇳🇴</h1>
   
    <p>
      Co-founder of <a href="https://twitter.com/gridsome">@gridsome</a> and <a href="https://twitter.com/uxthemes">@uxthemes</a> <br /> Building and designing web stuff.
    </p>

    <p class="links">
      <a href="https://gridsome.org/docs" target="_blank">Twitter</a>
      <a href="mailto:tommyvedvik@gmail.com" target="_blank">Contact</a>
    </p>

  </Layout>
</template>

<style>
.profile {
  border-radius: 999px;
}
.title {
  font-size: 1.6rem;
  font-weight: 500;
}
.links a {
  padding: 10px;
  display: inline-block;
}
</style>
