<script setup>
import { contactInfo } from "../data/items";

const copyrightText = "Copyright 2023, All rights reserved.";
const column1Heading = "About Sumnews.net";
const column1Text =
  "Sumnews.net is a platform designed to simplify news consumption by providing users with concise, summarized articles. Its goal is to help users stay informed without spending too much time on lengthy news pieces. Sumnews curates personalized news feeds based on users' interests and offers daily recaps of the most important stories, making it easy for users to catch up on key topics quickly. Whether you're busy or just looking for efficient news delivery, Sumnews aims to provide a seamless, time-saving way to stay up to date.";
const column2Heading = "Projects";
const column3Heading = "Services";
const column4Heading = "Contact";

const connectHeading = "Find us on Social Media";

const socialItems = [
  {
    link: "https://www.instagram.com/sumnews_net",
    icon: "icon-instagram",
  },
  {
    link: "https://x.com/sumnewsdotnet",
    icon: "icon-twitter",
  },
  {
    link: "https://www.linkedin.com/company/sumnews-net",
    icon: "icon-linkedin",
  }
];
</script>

<template>
  <div class="site-footer">
    <div class="footer-dots"></div>
    <div class="container">
      <div class="row">
        <div class="col-lg-4">
          <div class="widget">
            <h3>{{ column1Heading }}</h3>
            <p>{{ column1Text }}</p>
          </div>
          <!-- <div class="widget">
            <h3>{{ connectHeading }}</h3>
            <ul class="list-unstyled social">
              <li style="margin-right: 4px">
                <a :href="socialItems[0].link"><span :class="socialItems[0].icon"></span></a>
              </li>
              <li style="margin-right: 4px">
                <a :href="socialItems[1].link"><span :class="socialItems[1].icon"></span></a>
              </li>
              <li style="margin-right: 4px">
                <a :href="socialItems[2].link"><span :class="socialItems[2].icon"></span></a>
              </li>
            </ul>
          </div> -->
        </div>
        <div class="col-lg-2 ml-auto">
          <div class="widget">
            <h3>{{ column2Heading }}</h3>
            <ul class="list-unstyled float-left links">
              <li><a href="https://www.app.sumnews.net">Sumnew.net App</a></li>
            </ul>
          </div>
        </div>
        <!-- <div class="col-lg-2">
          <div class="widget">
            <h3>{{ column3Heading }}</h3>
            <ul class="list-unstyled float-left links">
              <li><a href="#">Architect</a></li>
              <li><a href="#">Interior Design</a></li>
              <li><a href="#">Landscape Design</a></li>
              <li><a href="#">Consultancy</a></li>
            </ul>
          </div>
        </div> -->
        <div class="col-lg-3">
          <div class="widget">
            <h3>{{ column4Heading }}</h3>
            <address>{{ contactInfo.address }}</address>
            <ul class="list-unstyled links mb-4">
              <!-- <li>
                <a :href="'tel://' + contactInfo.phone1">{{
                  contactInfo.phone1
                }}</a>
              </li>
              <li>
                <a :href="'tel://' + contactInfo.phone2">{{
                  contactInfo.phone2
                }}</a>
              </li> -->
              <li>
                <a :href="'mailto:' + contactInfo.email"><span>{{ contactInfo.supportEmail }}</span></a>
              </li>
            </ul>
          </div>
        </div>
      </div>
      <div class="row mt-5">
        <div class="col-12 text-center">
          <p>
            {{ copyrightText }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>
