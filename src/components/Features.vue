<script setup>
import feature1 from "../assets/images/features/feature-summarizedArticles.png";
import feature2 from "../assets/images/features/feature-dailyRecaps.png";
import feature3 from "../assets/images/features/feature-filterAndSearch.png";
import feature4 from "../assets/images/features/feature-fullCoverage.png";

const items = [
  {
    id: 1,
    name: "Summarized Articles",
    des: "Get concise summaries of the latest news articles, saving you time while keeping you informed",
  },
  {
    id: 2,
    name: "Daily Recaps",
    des: "Receive daily summaries of significant events, ensuring you never miss crucial updates",
  },
  {
    id: 3,
    name: "Filter and Search",
    des: "Search earch through a myriad of articles from different sources and genres and find the ones you're most interested in",
  },
  {
    id: 4,
    name: "Full Coverage",
    des: "Hear what other outlets have to same about the same event and get the full view of the story",
  },
];
const total = items.length;
</script>

<template>
  <div id="features-section" class="untree_co-section bg-light">
    <div class="container">
      <div class="row justify-content-center">
        <div class="col-lg-5 order-lg-2 js-custom-dots">
          <a href="#" class="service link horizontal d-flex active" data-aos="fade-left" data-aos-delay="0">
            <div class="service-icon color-1 mb-4">
              <!-- Summarized Articles Feature - svg -->
              <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 24 24">
                <g fill="none">
                  <path
                    d="m12.594 23.258l-.012.002l-.071.035l-.02.004l-.014-.004l-.071-.036q-.016-.004-.024.006l-.004.01l-.017.428l.005.02l.01.013l.104.074l.015.004l.012-.004l.104-.074l.012-.016l.004-.017l-.017-.427q-.004-.016-.016-.018m.264-.113l-.014.002l-.184.093l-.01.01l-.003.011l.018.43l.005.012l.008.008l.201.092q.019.005.029-.008l.004-.014l-.034-.614q-.005-.019-.02-.022m-.715.002a.02.02 0 0 0-.027.006l-.006.014l-.034.614q.001.018.017.024l.015-.002l.201-.093l.01-.008l.003-.011l.018-.43l-.003-.012l-.01-.01z" />
                  <path fill="currentColor"
                    d="M9.107 5.448c.598-1.75 3.016-1.803 3.725-.159l.06.16l.807 2.36a4 4 0 0 0 2.276 2.411l.217.081l2.36.806c1.75.598 1.803 3.016.16 3.725l-.16.06l-2.36.807a4 4 0 0 0-2.412 2.276l-.081.216l-.806 2.361c-.598 1.75-3.016 1.803-3.724.16l-.062-.16l-.806-2.36a4 4 0 0 0-2.276-2.412l-.216-.081l-2.36-.806c-1.751-.598-1.804-3.016-.16-3.724l.16-.062l2.36-.806A4 4 0 0 0 8.22 8.025l.081-.216zM11 6.094l-.806 2.36a6 6 0 0 1-3.49 3.649l-.25.091l-2.36.806l2.36.806a6 6 0 0 1 3.649 3.49l.091.25l.806 2.36l.806-2.36a6 6 0 0 1 3.49-3.649l.25-.09l2.36-.807l-2.36-.806a6 6 0 0 1-3.649-3.49l-.09-.25zM19 2a1 1 0 0 1 .898.56l.048.117l.35 1.026l1.027.35a1 1 0 0 1 .118 1.845l-.118.048l-1.026.35l-.35 1.027a1 1 0 0 1-1.845.117l-.048-.117l-.35-1.026l-1.027-.35a1 1 0 0 1-.118-1.845l.118-.048l1.026-.35l.35-1.027A1 1 0 0 1 19 2" />
                </g>
              </svg>
            </div>
            <div class="service-contents">
              <h3>{{ items[0].name }}</h3>
              <p>{{ items[0].des }}</p>
            </div>
          </a>
          <a href="#" class="service link horizontal d-flex" data-aos="fade-left" data-aos-delay="100">
            <div class="service-icon color-2 mb-4">
              <!-- Daily Recaps Feature - svg -->
              <svg class="bi bi-arrow-repeat" width="1em" height="1em" viewBox="0 0 16 16" fill="currentColor"
                xmlns="http://www.w3.org/2000/svg">
                <path fill-rule="evenodd"
                  d="M2.854 7.146a.5.5 0 0 0-.708 0l-2 2a.5.5 0 1 0 .708.708L2.5 8.207l1.646 1.647a.5.5 0 0 0 .708-.708l-2-2zm13-1a.5.5 0 0 0-.708 0L13.5 7.793l-1.646-1.647a.5.5 0 0 0-.708.708l2 2a.5.5 0 0 0 .708 0l2-2a.5.5 0 0 0 0-.708z" />
                <path fill-rule="evenodd"
                  d="M8 3a4.995 4.995 0 0 0-4.192 2.273.5.5 0 0 1-.837-.546A6 6 0 0 1 14 8a.5.5 0 0 1-1.001 0 5 5 0 0 0-5-5zM2.5 7.5A.5.5 0 0 1 3 8a5 5 0 0 0 9.192 2.727.5.5 0 1 1 .837.546A6 6 0 0 1 2 8a.5.5 0 0 1 .501-.5z" />
              </svg>
            </div>
            <div class="service-contents">
              <h3>{{ items[1].name }}</h3>
              <p>{{ items[1].des }}</p>
            </div>
          </a>
          <a href="#" class="service link horizontal d-flex" data-aos="fade-left" data-aos-delay="200">
            <div class="service-icon color-3 mb-4">
              <!-- Filter and Search Feature - svg -->
              <svg xmlns="http://www.w3.org/2000/svg" width="1em" height="1em" viewBox="0 0 15 15">
                <path fill="currentColor" fill-rule="evenodd"
                  d="M10 6.5a3.5 3.5 0 1 1-7 0a3.5 3.5 0 0 1 7 0m-.691 3.516a4.5 4.5 0 1 1 .707-.707l2.838 2.837a.5.5 0 0 1-.708.708z"
                  clip-rule="evenodd" />
              </svg>
            </div>
            <div class="service-contents">
              <h3>{{ items[2].name }}</h3>
              <p>{{ items[2].des }}</p>
            </div>
          </a>
          <a href="#" class="service link horizontal d-flex" data-aos="fade-left" data-aos-delay="300">
            <div class="service-icon color-4 mb-4">
              <!-- Full Coverage Feature - svg -->
              <svg class="bi bi-collection" width="1em" height="1em" viewBox="0 0 16 16" fill="currentColor"
                xmlns="http://www.w3.org/2000/svg">
                <path fill-rule="evenodd"
                  d="M14.5 13.5h-13A.5.5 0 0 1 1 13V6a.5.5 0 0 1 .5-.5h13a.5.5 0 0 1 .5.5v7a.5.5 0 0 1-.5.5zm-13 1A1.5 1.5 0 0 1 0 13V6a1.5 1.5 0 0 1 1.5-1.5h13A1.5 1.5 0 0 1 16 6v7a1.5 1.5 0 0 1-1.5 1.5h-13zM2 3a.5.5 0 0 0 .5.5h11a.5.5 0 0 0 0-1h-11A.5.5 0 0 0 2 3zm2-2a.5.5 0 0 0 .5.5h7a.5.5 0 0 0 0-1h-7A.5.5 0 0 0 4 1z" />
              </svg>
            </div>
            <div class="service-contents">
              <h3>{{ items[3].name }}</h3>
              <p>{{ items[3].des }}</p>
            </div>
          </a>
        </div>
        <div class="col-lg-7">
          <div class="img-shadow">
            <div class="owl-single no-dots owl-carousel">
              <div class="item">
                <span class="number">{{ items[0].id }}/{{ total }}</span>
                <img :src="feature1" alt="Image" class="img-fluid" />
              </div>
              <div class="item">
                <span class="number">{{ items[1].id }}/{{ total }}</span>
                <img :src="feature2" alt="Image" class="img-fluid" />
              </div>
              <div class="item">
                <span class="number">{{ items[2].id }}/{{ total }}</span>
                <img :src="feature3" alt="Image" class="img-fluid" />
              </div>
              <div class="item">
                <span class="number">{{ items[3].id }}/{{ total }}</span>
                <img :src="feature4" alt="Image" class="img-fluid" />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.img-fluid {
  width: auto !important;
  aspect-ratio: 9 / 16;
  max-height: 625.6px;
}

@media (min-width: 992px) {
  .col-lg-7 {
    flex: 0 0 42%;
    max-width: 352px;
  }
}
</style>