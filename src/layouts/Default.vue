<template>
  <div class="layout">
    <div class="content">
      <div class="content__inner">
        <slot/>
      </div>
    </div>
    <g-image class="bg-layer" src="../assets/bg.gif" />
    <div class="bg-layer"></div>
  </div>
</template>

<static-query>
query {
  metaData {
    siteName
  }
}
</static-query>

<style>
html {
  padding:0;
  margin:0;
}
body {
  font-family: -apple-system,system-ui,BlinkMacSystemFont,"Segoe UI",Roboto,"Helvetica Neue",Arial,sans-serif;
  margin:0;
  padding:0;
  line-height: 1.6;
  background-color: #242f41;
  color: rgba(255,255,255,.7);
}

.content {
  z-index: 11;
  position: relative;
  min-height: 100vh;
  margin: 0 auto;
  max-width: 500px;
  display: flex;
  align-items: center;
  text-align: center;
}

.content__inner {
  padding: 5%;
  flex:1;
}

.bg-layer {
  position: fixed;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  object-fit: cover;
  object-position: 30% 30%;
  width: 100%;
  height: 100%;
  background: #242f41;
  opacity:0.5;
  z-index: 10;
}

a, 
a:visited {
  color:#FFF;
  text-decoration: none;
}

a:hover {
  opacity: .7;
}
</style>
