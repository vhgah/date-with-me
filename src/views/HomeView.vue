<script setup lang="ts"></script>

<template>
  <div class="container">
    <header>
      <div class="logo">HoangAnh</div>
      <div class="title">Date with me</div>
    </header>
    <img src="../assets/images/demo.webp" alt="image" class="content_image" />
    <div class="content_description">
      <p>
        Datewithme is a platform designed to help you create the most romantic and memorable date
        plans.
      </p>
      <p>
        We understand that planning the perfect date can be challenging, so we’ve developed an
        easy-to-use tool to help you effortlessly organize special outings with your loved ones.
      </p>

      <RouterLink to="hongmo" class="w-fit font-medium text-blue-600 hover:underline">
        See a demo
      </RouterLink>
    </div>
    <div class="widget">
      <div class="widget-item">
        <a target="_blank" href="https://www.facebook.com/vhgah"
          ><svg xmlns="http://www.w3.org/2000/svg" role="img" viewBox="0 0 24 24" class="facebook">
            <title>Facebook</title>
            <path
              d="M19 2H5a3 3 0 0 0-3 3v14a3 3 0 0 0 3 3h7.66v-7.37h-2.4V10.8h2.4V8.36c0-2.37 1.45-3.66 3.74-3.66h1.77v2.96h-1.23c-.41 0-.97.2-1.13.88-.12.45-.12.92-.12 1.38v1.78h2.41l-.31 2.47h-2.1V22H19a3 3 0 0 0 3-3V5a3 3 0 0 0-3-3z"
            ></path></svg
        ></a>
      </div>
      <div class="widget-item">
        <a target="_blank" href="https://github.com/vhgah"
          ><svg xmlns="http://www.w3.org/2000/svg" role="img" viewBox="0 0 24 24" class="github">
            <title>Github</title>
            <path
              d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-4.466 19.59c-.405.078-.534-.171-.534-.384v-2.195c0-.747-.262-1.233-.55-1.481 1.782-.198 3.654-.875 3.654-3.947 0-.874-.312-1.588-.823-2.147.082-.202.356-1.016-.079-2.117 0 0-.671-.215-2.198.82-.64-.18-1.324-.267-2.004-.271-.68.003-1.364.091-2.003.269-1.528-1.035-2.2-.82-2.2-.82-.434 1.102-.16 1.915-.077 2.118-.512.56-.824 1.273-.824 2.147 0 3.064 1.867 3.751 3.645 3.954-.229.2-.436.552-.508 1.07-.457.204-1.614.557-2.328-.666 0 0-.423-.768-1.227-.825 0 0-.78-.01-.055.487 0 0 .525.246.889 1.17 0 0 .463 1.428 2.688.944v1.489c0 .211-.129.459-.528.385-3.18-1.057-5.472-4.056-5.472-7.59 0-4.419 3.582-8 8-8s8 3.581 8 8c0 3.533-2.289 6.531-5.466 7.59z"
            ></path></svg
        ></a>
      </div>
    </div>
    <footer>
      <p class="footer-left">Copyright © Datewithme</p>
      <p class="footer-right">HoangAnh</p>
    </footer>
  </div>
</template>
<style scoped>
.container {
  font-family: 'Be Vietnam Pro', sans-serif;
  font-size: 24px;
  line-height: 1.2em;
  align-items: center;
  background-color: #fff;
  display: flex;
  flex-direction: column;
  flex-wrap: nowrap;
  gap: 60px;
  height: min-content;
  justify-content: flex-start;
  overflow: hidden;
  padding: 100px 50px;
  position: relative;
  min-height: 100vh;
  max-width: 900px;
  margin: 0 auto;
}

@media (max-width: 809px) {
  .container {
    padding: 40px 30px;
  }
}

header {
  align-items: flex-start;
  display: flex;
  flex: none;
  flex-direction: column;
  flex-wrap: nowrap;
  gap: 15px;
  height: min-content;
  justify-content: flex-start;
  max-width: 900px;
  overflow: visible;
  padding: 0;
  position: relative;
  width: 100%;
}

.logo {
  outline: none;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  flex-shrink: 0;
  transform: none;
  color: #b2b2b2;
}

.title {
  outline: none;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  flex-shrink: 0;
  opacity: 1;
  transform: none;
  color: #000;
  font-size: 32px;
  font-weight: 500;
  font-family: 'Be Vietnam Pro', 'Be Vietnam Pro Placeholder', sans-serif;
}

.content_image {
  border-radius: 20px;
}

img {
  display: block;
  width: 100%;
  height: 100%;
  border-radius: inherit;
  object-position: center;
  object-fit: cover;
  image-rendering: auto;
}

.content_description {
  outline: none;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  flex-shrink: 0;
  transform: none;
  font-size: 18px;
  line-height: 1.6em;
  font-weight: 350;
}

svg {
  fill: currentColor;
  color: rgb(107 114 128);
  transition: all 0.2s ease-in-out;
}

.facebook {
  height: 40px;
  width: 40px;
}

.github {
  height: 35px;
  width: 35px;
}

.widget {
  display: flex;
  flex-direction: row;
  justify-content: center;
  gap: 20px;
}

.widget-item {
  display: flex;
  align-items: center;
  justify-content: center;
}

.widget-item:hover svg {
  color: rgb(17 24 39);
}

footer {
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 100%;
  width: 100%;
}

.footer-left {
  font-size: 14px;
  font-weight: 400;
  color: #b2b2b2;
}

.footer-right {
  font-size: 14px;
  font-weight: 400;
  color: #b2b2b2;
}
</style>
