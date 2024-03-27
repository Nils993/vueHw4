<template>
  <div id="app">
    <HeaderPage />
    <section class="intro">
      <div class="intro-info">
        <h2 class="intro__title">Articles & News</h2>
        <p class="intro__text">Home / Blog</p>
      </div>
    </section>
    <section class="latestPost center">
      <h2 class="latestPost__heading">Latest Post</h2>
      <div class="latestPost-wrap">
        <div class="latestPost__img"></div>
        <div class="latestPost-info">
          <h3 class="latestPost__title">
            Low Cost Latest Invented Interior Designing Ideas
          </h3>
          <div class="latestPost__text">
            <p>
              Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpis
              dignissim maximus.posuere in.Contrary to popular belief.
            </p>
            <p>
              Lorem Ipsum is not simply random text. It has roots in a piece of
              classica.
            </p>
          </div>

          <div class="latestPost-wrap__btn">
            <p class="latestPost__data">26 December,2022</p>
            <button class="projects-item__but projects-item__but_blog">
              <svg
                width="10"
                height="20"
                viewBox="0 0 10 20"
                fill="none"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  d="M1 19L9 10L1 1"
                  stroke="#292F36"
                  stroke-width="2"
                  stroke-linecap="round"
                  stroke-linejoin="round"
                />
              </svg>
            </button>
          </div>
        </div>
      </div>
    </section>
    <section class="blog center">
      <h3 class="blog-heading__title">Articles & News</h3>
      <div class="blog-cards_page2">
        <div v-for="article in articles" class="blog-card blog-card_page2">
          <img
            class="blog-card__back"
            width="380"
            :src="article.image"
            alt=""
          />
          <p class="blog-card__tag">{{ article.tag }}</p>

          <div class="blog-card-info">
            <h3 class="blog-card__title">{{ article.title }}</h3>
            <div class="blog-card-wraper-but">
              <p class="blog-card__date">{{ article.date }}</p>
              <button class="projects-item__but projects-item__but_blog">
                <svg
                  width="10"
                  height="20"
                  viewBox="0 0 10 20"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M1 19L9 10L1 1"
                    stroke="#292F36"
                    stroke-width="2"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                </svg>
              </button>
            </div>
          </div>
        </div>
      </div>
      <div class="blog-page">
        <button class="projects-item__but blog-page__but">01</button>
        <button class="projects-item__but blog-page__but">02</button>
        <button class="projects-item__but blog-page__but">03</button>

        <button class="projects-item__but blog-page__but">
          <svg
            width="10"
            height="20"
            viewBox="0 0 10 20"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M1 19L9 10L1 1"
              stroke="#292F36"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
            />
          </svg>
        </button>
      </div>
    </section>
    <FooterPage />
  </div>
</template>

<script>
import HeaderPage from "./components/HeaderPage.vue";
import FooterPage from "./components/FooterPage.vue";

export default {
  name: "Page2",
  components: {
    HeaderPage,
    FooterPage,
  },
  data() {
    return {
      articles: [
        {
          tag: "Kitchan Design",
          title: "Let’s Get Solution For Building Construction Work",
          date: "26 December,2022",
          image: "./img/cart1.png",
        },
        {
          tag: "Living Design",
          title: "Low Cost Latest Invented Interior Designing Ideas.",
          date: "22 December,2022",
          image: "./img/cart2.png",
        },
        {
          tag: "Interior Design",
          title: "Best For Any Office & Business Interior Solution",
          date: "25 December,2022",
          image: "./img/cart3.png",
        },
        {
          tag: "Kitchan Design",
          title: "Let’s Get Solution For Building Construction Work",
          date: "26 December,2022",
          image: "./img/cart1.png",
        },
        {
          tag: "Living Design",
          title: "Low Cost Latest Invented Interior Designing Ideas.",
          date: "22 December,2022",
          image: "./img/cart2.png",
        },
        {
          tag: "Interior Design",
          title: "Best For Any Office & Business Interior Solution",
          date: "25 December,2022",
          image: "./img/cart3.png",
        },
      ],
    };
  },
};
</script>

<style>
* {
  margin: 0;
  padding: 0;
}

body {
  font-family: "Jost", sans-serif;
  font-family: "DM Serif Display", serif;
}

.center {
  padding-left: calc(50% - 600px);
  padding-right: calc(50% - 600px);
}

a {
  text-decoration: none;
}
.details-banner {
  background-image: url(./assets/DetailsBaner.png);
  height: 350px;
  background-repeat: no-repeat;
  background-position: center;
}
</style>
