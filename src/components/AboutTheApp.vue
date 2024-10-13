<script setup>
import { themeColor } from "../data/items";
import personPhoto from "../assets/images/person_1.jpg";
import mainPhoto from "../assets/images/service1.jpg";

const service1Heading = "About the App";
const service1SubHeading = "Welcome to Sumnews";
const service1Quote =
  '"Sumnews has transformed how I stay updated. It’s incredibly easy to use and keeps me informed without the hassle. The perfect solution for anyone who wants quick, summarized news on the go."';

const websiteLink = "https://app.sumnews.net";
const googlePlayLink = "";
const appStoreLink = ""
const personName = "James A.";
const designation = "Satisfied User";
function youtubeVideoUrl() {
  const youtubeVideoId = "FzRH7y3LbQE";
  return `https://www.youtube.com/watch?v=${youtubeVideoId}&amp;t=9s`;
}
</script>
<template>
  <div class="untree_co-section" id="about-the-app-section">
    <div class="container">
      <div class="row justify-content-between">
        <div class="col-lg-4">
          <span class="caption" data-aos="fade-up" data-aos-delay="0" :style="[{ color: themeColor }]">{{
            service1Heading }}</span>
          <h3 class="heading mb-4" data-aos="fade-up" data-aos-delay="100">
            {{ service1SubHeading }}
          </h3>
          <div class="mb-4" data-aos="fade-up" data-aos-delay="200">
            <p>
              In a world filled with information, it’s easy to feel overwhelmed. That’s where Sumnews.net comes in.
              We’re here to simplify your news experience by providing you with the most important headlines, summarized
              for quick and easy consumption. Whether you're on the go or just want the facts without the fluff,
              Sumnews.net delivers personalized news tailored to your interests—making it easier to stay informed and in
              control of your time.
            </p>
          </div>
          <div class="mb-4" data-aos="fade-up" data-aos-delay="300">
            <div class="untree_co-testimonial d-flex">
              <div class="text">
                <blockquote>
                  {{ service1Quote }}
                </blockquote>
                <div class="author d-flex">
                  <div class="pic mr-3">
                    <img :src="personPhoto" alt="Image" class="img-fluid" />
                  </div>
                  <div>
                    <strong class="d-block">{{ personName }}</strong><span class="d-block">{{ designation }}</span>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-lg-7 align-items-center justify-content-center row" data-aos="fade-up" data-aos-delay="400">
          <div class="video-container">
            <iframe width="560" height="315"
              src="https://www.youtube.com/embed/BggyW8UGmxw?si=yy_ddF79tyjoD3lQ&autoplay=1&mute=1"
              title="YouTube video player" frameborder="0"
              allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
              referrerpolicy="strict-origin-when-cross-origin" allowfullscreen>
            </iframe>
          </div>
        </div>
        <!-- <div class="col-lg-7" data-aos="fade-up" data-aos-delay="400">
          <a :href="youtubeVideoUrl()" class="btn-video" data-fancybox>
            <span class="wrap-icon-play">
              <svg class="bi bi-play-fill" width="1em" height="1em" viewBox="0 0 16 16" fill="currentColor"
                xmlns="http://www.w3.org/2000/svg">
                <path
                  d="M11.596 8.697l-6.363 3.692c-.54.313-1.233-.066-1.233-.697V4.308c0-.63.692-1.01 1.233-.696l6.363 3.692a.802.802 0 0 1 0 1.393z" />
              </svg>
            </span>
            <img :src="mainPhoto" alt="Image" class="img-fluid img-shadow" />
          </a>
        </div> -->
      </div>
    </div>
  </div>
</template>
