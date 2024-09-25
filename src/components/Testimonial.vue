<script setup>
import { themeColor } from "../data/items";

const heading = "Testimonials";
const subHeading = "Our Customers Feedback";
const testimonials = [
  {
    name: "Michael T.",
    designation: "Entreprenuer",
    singleLiner: "Sumnew.net has been a game-changer for me",
    quote:
      `"As someone who doesn't have time to sift through countless news articles every day, Sumnews.net has been a game- changer for me.The daily recaps give me everything I need to know in just a few minutes, and I love how the summaries are always right on point.I feel more informed without having to invest hours of my time—definitely recommend this to anyone who values efficiency and staying up - to - date."`,
    photo: "images/person_1.jpg",
  },
  {
    name: "Sarah L.",
    designation: "Marketing Manager",
    singleLiner: "Finally, a curated feed that actually understands what I care about",
    quote:
      `"I used to waste time scrolling through multiple news sites that didn't align with my interests. Sumnews.net’s curated feed solves that problem by delivering the news I actually care about. Whether it's politics or world news, it's all relevant to me. Other platforms don't come close in terms of personalization—it's honestly become my go-to source every day."`,
    photo: "images/person_2.jpg",
  },
  {
    name: "David R.",
    designation: "IT Specialist",
    singleLiner: "I dont' know how I stayed informed before Sumnews.net",
    quote:
      `"With so much noise in the news today, it was hard to find a platform that cuts to the chase. Sumnews.net does just that. The daily recaps are amazing—they sum up everything important so I never miss out. Compared to other news sources, which bombard you with endless content, this app respects my time while keeping me well-informed. Highly recommend!"`,
    photo: "images/person_3.jpg",
  },
];
</script>

<template>
  <div class="untree_co-section" id="testimonials-section">
    <div class="container">
      <div class="row">
        <div class="col-lg-4 mb-5 text-center text-lg-left mb-lg-0" data-aos="fade-up" data-aos-delay="0">
          <div class="mb-4">
            <span class="caption" :style="[{ color: themeColor }]">{{
              heading
            }}</span>
            <h2 class="heading">{{ subHeading }}</h2>
          </div>
          <div>
            <a href="#" class="js-custom-prev-v2 cusotm-slider-nav custom-prev" style="margin-right: 5px">
              <span>
                <svg class="bi bi-arrow-left" width="1em" height="1em" viewBox="0 0 16 16" fill="currentColor"
                  xmlns="http://www.w3.org/2000/svg">
                  <path fill-rule="evenodd"
                    d="M5.854 4.646a.5.5 0 0 1 0 .708L3.207 8l2.647 2.646a.5.5 0 0 1-.708.708l-3-3a.5.5 0 0 1 0-.708l3-3a.5.5 0 0 1 .708 0z" />
                  <path fill-rule="evenodd" d="M2.5 8a.5.5 0 0 1 .5-.5h10.5a.5.5 0 0 1 0 1H3a.5.5 0 0 1-.5-.5z" />
                </svg>
              </span>
            </a>
            <a href="#" class="js-custom-next-v2 cusotm-slider-nav custom-next">
              <span>
                <svg class="bi bi-arrow-right" width="1em" height="1em" viewBox="0 0 16 16" fill="currentColor"
                  xmlns="http://www.w3.org/2000/svg">
                  <path fill-rule="evenodd"
                    d="M10.146 4.646a.5.5 0 0 1 .708 0l3 3a.5.5 0 0 1 0 .708l-3 3a.5.5 0 0 1-.708-.708L12.793 8l-2.647-2.646a.5.5 0 0 1 0-.708z" />
                  <path fill-rule="evenodd" d="M2 8a.5.5 0 0 1 .5-.5H13a.5.5 0 0 1 0 1H2.5A.5.5 0 0 1 2 8z" />
                </svg>
              </span>
            </a>
          </div>
        </div>
        <div class="col-lg-8" data-aos="fade" data-aos-delay="200">
          <div class="owl-2-slider owl-carousel">
            <div class="item">
              <div class="untree_co-testimonial d-flex">
                <div class="text">
                  <p class="single-liner">
                    {{ testimonials[0].singleLiner }}
                  </p>
                  <blockquote>
                    {{ testimonials[0].quote }}
                  </blockquote>
                  <div class="author d-flex">
                    <div class="pic mr-3">
                      <img :src="testimonials[0].photo" alt="Image" class="img-fluid" />
                    </div>
                    <div>
                      <strong class="d-block">{{ testimonials[0].name }}</strong><span class="d-block">{{
                        testimonials[0].designation
                      }}</span>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div class="item">
              <div class="untree_co-testimonial d-flex">
                <div class="text">
                  <p class="single-liner">
                    {{ testimonials[1].singleLiner }}
                  </p>
                  <blockquote>
                    {{ testimonials[1].quote }}
                  </blockquote>
                  <div class="author d-flex">
                    <div class="pic mr-3">
                      <img :src="testimonials[1].photo" alt="Image" class="img-fluid" />
                    </div>
                    <div>
                      <strong class="d-block">{{ testimonials[1].name }}</strong><span class="d-block">{{
                        testimonials[1].designation
                      }}</span>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div class="item">
              <div class="untree_co-testimonial d-flex">
                <div class="text">
                  <p class="single-liner">
                    {{ testimonials[2].singleLiner }}
                  </p>
                  <blockquote>
                    {{ testimonials[2].quote }}
                  </blockquote>
                  <div class="author d-flex">
                    <div class="pic mr-3">
                      <img :src="testimonials[2].photo" alt="Image" class="img-fluid" />
                    </div>
                    <div>
                      <strong class="d-block">{{ testimonials[2].name }}</strong><span class="d-block">{{
                        testimonials[2].designation
                      }}</span>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.single-liner {
  font-size: 18px;
  font-style: italic;
  color: black;
  background: plum;
  display: inline;
  /* Ensures the background applies only to the text */
  padding: 0 4px;
  /* Optional: Adds a small padding to mimic a highlight effect */
  border-radius: 4px;
}
</style>