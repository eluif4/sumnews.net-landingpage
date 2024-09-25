<script setup>
import Header from "./components/Header.vue";
import Hero from "./components/Hero.vue";
import AboutTheApp from "./components/AboutTheApp.vue";
import Features from "./components/Features.vue";
import Feature from "./components/Feature.vue";
import Pricing from "./components/Pricing.vue";
import Advantage from "./components/Advantage.vue";
import Testimonial from "./components/Testimonial.vue";
import About from "./components/About.vue";
import Blog from "./components/Blog.vue";
import Contact from "./components/Contact.vue";
import Footer from "./components/Footer.vue";
</script>

<template>
  <Header />
  <Hero />
  <AboutTheApp />
  <Features />
  <!-- <Feature /> -->
  <!-- <Pricing /> -->
  <!-- <Pricing /> -->
  <!-- <Advantage /> -->
  <Testimonial />
  <About />
  <!-- <Blog /> -->
  <Contact />
  <Footer />
</template>

<style>
.bold {
  color: var(--main-color);
  font-weight: bold;
  transition: all 0.3s ease;
  cursor: pointer;
}

.quote {
  background-color: plum;
  border-radius: 4px;
  color: black;
  font-weight: bold;
  transition: all 0.3s ease;
}

.ul-red-x li::before {
  content: '✖';
  /* Red X */
  color: red;
  margin-right: 10px;
  /* Spacing between the X and the text */
  font-size: 1.2em;
  /* Adjust size if needed */
}
</style>