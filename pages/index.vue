<template>
  <section class="container">
    <div>
      <logo />
      <cld-image public-id="jigglypuff" width="100" height="100" cloudName="mayashavin">
      <cld-transformation effect="grayscale" angle="45" crop="scale"/>
    </cld-image>
    <!-- <cld-video cloudName="demo" publicId="face_top">
          <cld-poster publicId="small_dinosaur" />
        </cld-video> -->
    <div class="test">
          <cld-context cloudName="demo" secure=true>
              <cld-image publicId="face_top" quality="80" />
          </cld-context>
        </div>
    <cld-context cloud-name="demo" secure=true>
      <div><cld-image public-id="face_top"/></div>
    </cld-context>
    <cld-image publicId="sample" cloudName="demo">
      <div>
        <cld-transformation width="100" crop="scale" />
        <cld-transformation width="200" crop="pad" />
        <cld-transformation angle="30" />
      </div>
    </cld-image>
      <h1 class="title">
        nuxt-app
      </h1>
      <h2 class="subtitle">
        My outstanding Nuxt.js project
      </h2>
      <div class="links">
        <a
          href="https://nuxtjs.org/"
          target="_blank"
          class="button--green"
        >Documentation</a>
        <a
          href="https://github.com/nuxt/nuxt.js"
          target="_blank"
          class="button--grey"
        >GitHub</a>
      </div>
    </div>
  </section>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
