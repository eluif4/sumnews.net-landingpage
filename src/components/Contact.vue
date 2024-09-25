<script setup>
import { themeColor, contactInfo } from "../data/items";

const heading = "Get In Touch";
const subHeading = "We're Here to Hear From You!";
const contactInfoHeading = "Contact Information";
const buttonSendMessage = "Send Message";
const labels = {
  firstName: "First Name",
  lastName: "Last Name",
  email: "Email Address",
  message: "Message",
};

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
  <div class="untree_co-section" id="contact-section">
    <div class="container">
      <div class="row mb-4" data-aos="fade-up" data-aos-delay="0">
        <div class="col-12 text-center">
          <h2 class="heading">{{ heading }}</h2>
          <p>{{ subHeading }}</p>
        </div>
      </div>
      <div class="row">
        <div class="col-lg-7">
          <h3 class="bold">Generl Inquiries</h3>
          <p>Have questions, feedback, or just want to say hello? We'd love to hear from you! You can reach us via email
            at <a :href="'mailto:' + contactInfo.infoEmail">info@sumnews.net</a></p>
          <h3 class="bold">Customers Support</h3>
          <p>
            If you require assistance or have specific queries related to the Sumnews.net platform, our customer
            support team is here to help. Please email us at <a
              :href="'mailto:' + contactInfo.supportEmail">support@sumnews.net</a>, and we'll get back to you as soon as
            possible.
          </p>
          <h3 class="bold">We Value Your Feedback</h3>
          <p>
            Your feedback is essential to us. Whether it's a suggestion for improvement or a positive experience you'd
            like to share, we appreciate your input. Together, let's make Sumnews.net even better! Thank you for being a
            part of our community.
          </p>
        </div>
        <!-- <div class="col-lg-7">
          <form class="contact-form" data-aos="fade-up" data-aos-delay="100">
            <div class="row">
              <div class="col-6">
                <div class="form-group">
                  <label class="" for="fname">{{ labels.firstName }}</label>
                  <input type="text" class="form-control" id="fname" />
                </div>
              </div>
              <div class="col-6">
                <div class="form-group">
                  <label class="" for="lname">{{ labels.lastName }}</label>
                  <input type="text" class="form-control" id="lname" />
                </div>
              </div>
            </div>
            <div class="form-group">
              <label class="" for="email">{{ labels.email }}</label>
              <input type="email" class="form-control" id="email" />
            </div>
            <div class="form-group">
              <label class="" for="message">{{ labels.message }}</label>
              <textarea
                name=""
                class="form-control"
                id="message"
                cols="30"
                rows="5"
              ></textarea>
            </div>
            <button
              type="submit"
              class="btn btn-primary"
              :style="[
                { backgroundColor: themeColor },
                { borderColor: themeColor },
              ]"
            >
              {{ buttonSendMessage }}
            </button>
          </form>
        </div> -->
        <div class="col-lg-4 ml-auto" data-aos="fade-up" data-aos-delay="200">
          <h3 class="h5 mb-4">{{ contactInfoHeading }}</h3>
          <!-- <address class="text-black d-flex">
            <span class="mt-1 icon-room mr-2"></span><span>{{ contactInfo.address }}</span>
          </address> -->
          <ul class="list-unstyled ul-links mb-4">
            <!-- <li>
              <a :href="'tel://' + contactInfo.phone1" class="d-flex"><span class="mt-1 icon-phone mr-2"></span><span>{{
                contactInfo.phone1 }}</span></a>
            </li>
            <li>
              <a :href="'tel://' + contactInfo.phone2" class="d-flex"><span class="mt-1 icon-phone mr-2"></span><span>{{
                contactInfo.phone2 }}</span></a>
            </li> -->
            <li>
              <a :href="'mailto:' + contactInfo.infoEmail" class="d-flex"><span
                  class="mt-1 icon-envelope mr-2"></span><span>{{ contactInfo.infoEmail }}</span></a>
            </li>
            <li>
              <a :href="'mailto:' + contactInfo.supportEmail" class="d-flex"><span
                  class="mt-1 icon-envelope mr-2"></span><span>{{ contactInfo.supportEmail }}</span></a>
            </li>
            <li>
              <a :href="[contactInfo.website]" target="_blank" class="d-flex"><span
                  class="mt-1 icon-globe mr-2"></span><span>{{ contactInfo.website }}</span></a>
            </li>
          </ul>
          <h3 class="h5 mb-4">Find us on Social Media</h3>
          <div class="widget social-widgets">
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
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.social-widgets ul {
  display: flex;
  flex-direction: row;
  /* justify-content: center; */
  transition: transform 0.3s;
}

.social-widgets li a {
  /* display: inline-block; */
  width: 30px;
  height: 30px;
  position: relative;
  background: #777;
  border-radius: 50%;
  color: #ffffff;
  margin: auto;
}

.social-widgets a {
  display: flex;
  justify-content: center;
  align-items: center;
}

.social-widgets li a:hover {
  background: #739eff;
  color: #ffffff;
}
</style>