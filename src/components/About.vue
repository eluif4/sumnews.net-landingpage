<script setup>
import { themeColor } from "../data/items";
import mainPhoto from "../assets/images/about2.svg";

const heading = "About";
const subHeading = "About Us";
const totalMembers = "50";
const totalTeam = "20";
</script>

<template>
  <div class="untree_co-section" id="about-section">
    <div class="container">
      <div class="row justify-content-between">
        <div class="col-lg-8" data-aos="fade-up" data-aos-delay="100">
          <img :src="mainPhoto" alt="Image" class="img-fluid" style="margin: 24% 0" />
        </div>
        <div class="col-lg-4">
          <div class="mb-4" data-aos="fade-up" data-aos-delay="0">
            <span class="caption" :style="[{ color: themeColor }]">{{
              heading
            }}</span>
            <h2 class="heading">{{ subHeading }}</h2>
          </div>
          <div class="mb-4" data-aos="fade-up" data-aos-delay="100">
            <h3 class="bold">Our Mission</h3>
            <p>
              At Sumnews.net, we believe in making information more accessible and convenient for everyone. Our mission
              is to empower users with succinct and relevant news summaries, helping them stay informed in today's
              fast-paced world.
            </p>
            <h3 class="bold">Our Commiment</h3>
            <p>
              We are dedicated to refining and enhancing our platform continuously. User feedback is invaluable to us,
              and we actively incorporate suggestions to improve the quality of our service
            </p>
          </div>
          <h3 class="bold">What set's us apart?</h3>
          <ul class="list-unstyled ul-check primary mb-4" data-aos="fade-up" data-aos-delay="200">
            <li>Automatic Summarization Technology</li>
            <li>Diverse News Sources</li>
            <li>User-Centric Design</li>
          </ul>
          <!-- <div class="row count-numbers">
            <div class="col-lg-6" data-aos="fade-up" data-aos-delay="0">
              <span class="counter d-block"><span :data-number="totalMembers">{{ totalMembers
                  }}</span><span>M</span></span>
              <span class="caption-2">Members</span>
            </div>
            <div class="col-lg-6" data-aos="fade-up" data-aos-delay="100">
              <span class="counter d-block"><span :data-number="totalTeam">{{ totalTeam }}</span><span></span></span>
              <span class="caption-2">Team</span>
            </div>
          </div> -->
        </div>
      </div>
    </div>
  </div>
</template>