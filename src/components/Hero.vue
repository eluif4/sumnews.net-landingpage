<script setup>
import mainPhoto from "../assets/images/phonetemplate.svg";
import { themeColor } from "../data/items";

const heroHeading = "It's not just News";
const buttonSeeFeature = "See Features";
const buttonPricing = "Social Media";
</script>

<template>
  <div class="untree_co-hero" id="home-section">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-12">
          <div class="dots"></div>
          <div class="row align-items-center phone-mockup">
            <div class="col-lg-7 ml-auto order-lg-2" data-aos="fade-right" data-aos-delay="400">
              <img :src="mainPhoto" alt="Image" class="img-fluid phone" />
            </div>
            <div class="col-lg-5">
              <h1 class="heading" data-aos="fade-up" data-aos-delay="0">
                {{ heroHeading }}
                <br>
                It's
                <span class="bold">Sumnews</span>
              </h1>
              <div class="excerpt" data-aos="fade-up" data-aos-delay="100">
                <p>
                  Sumnews.net delivers the latest news in <span class="bold">concise, easy-to-read summaries</span>,
                  helping you stay updated
                  without the hassle of reading long articles.
                  Whether you're catching up on <span class="bold">politics, international
                  affairs,</span> or <span class="bold">trending headlines</span>, Sumnews.net gets right to the point—saving you time and keeping you
                  informed. 
                  <!-- Let us handle the details, so you can stay in the know, no matter how busy life gets. -->
                </p>
              </div>
              <p data-aos="fade-up" data-aos-delay="200">
                <a href="#features-section" class="btn btn-primary smoothscroll" style="margin-right: 5px" :style="[
                  { background: themeColor },
                  { borderColor: themeColor },
                ]">{{ buttonSeeFeature }}</a>
                <a href="#pricing-section" class="btn btn-outline-primary smoothscroll pricing"
                  :style="[{ color: themeColor }, { borderColor: themeColor }]">{{ buttonPricing }}</a>
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.pricing:hover {
  color: #fff !important;
}

.phone {
  height: 400px;
  aspect-ratio: 9 / 16;
}

.phone-container {
  gap: 40px;
}

.bold {
  color: var(--main-color);
  font-weight: bold;
  transition: all 0.3s ease;
  cursor: pointer;
}

.bold:hover {
  /* font-size: calc(100% + 4px); Add 4px to the current font size */
  color: #62FEBD;
}
</style>
