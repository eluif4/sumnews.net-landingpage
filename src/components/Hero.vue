<script setup>
import mainPhoto from "../assets/images/phonefeed.svg";
import { themeColor } from "../data/items";

const heroHeading = "It's not just News";
const buttonSeeFeature = "See Features";
const buttonApp = "Open the App";
</script>

<template>
  <div class="untree_co-hero" id="home-section">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-12">
          <div class="dots"></div>
          <div class="row align-items-center phone-mockup">
            <div class="order-lg-2" data-aos="fade-right" data-aos-delay="400">
              <img :src="mainPhoto" alt="Image" class="img-fluid phone" />
            </div>
            <div class="col-lg-8">
              <h1 class="heading" data-aos="fade-up" data-aos-delay="0">
                {{ heroHeading }}
                <br>
                It's
                <a href="https://www.app.sumnews.net"><span class="bold">Sumnews</span></a>
              </h1>
              <div class="excerpt" data-aos="fade-up" data-aos-delay="100">
                <p>
                  Sumnews.net delivers the latest news in <span class="quote">concise, easy-to-read summaries</span>,
                  helping you stay updated
                  without the hassle of reading long articles.
                  Whether you're catching up on <span class="quote">politics, international
                    affairs,</span> or <span class="quote">trending headlines</span>, Sumnews.net gets right to the
                  point—saving you time and keeping you
                  informed.
                  <!-- Let us handle the details, so you can stay in the know, no matter how busy life gets. -->
                </p>
              </div>
              <p data-aos="fade-up" data-aos-delay="200">
                <!-- <a id="btn-features" href="#features" class="btn btn-primary smoothscroll" style="margin: 0 5px 5px 0"
                  :style="[
                    { background: themeColor },
                    { borderColor: themeColor },
                  ]">{{ buttonSeeFeature }}</a> -->
                <a id="btn-app" href="https://www.app.sumnews.net" class="btn smoothscroll pricing"
                  style="margin: 0 5px 5px 0" :style="[{ color: themeColor }, { borderColor: themeColor }]">{{ buttonApp
                  }}</a>
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.row {
  display: flex;
  margin: 0;
  flex-direction: row;
  gap: 40px;
  flex-wrap: wrap;
  align-content: center;
  justify-content: center;
}

.pricing:hover {
  color: #fff !important;
  background-color: var(--main-color);
}

.phone {
  height: 450px;
  aspect-ratio: 9 / 16;
}

.phone-container {
  gap: 40px;
}

.bold:hover {
  /* font-size: calc(100% + 4px); Add 4px to the current font size */
  color: #62FEBD;
}
</style>
