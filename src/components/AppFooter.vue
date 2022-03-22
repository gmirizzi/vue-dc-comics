<template>
  <footer>
    <div class="container">
      <div id="links">
        <section v-for="section in sections" :key="section.title">
          <h1>{{ section.title }}</h1>
          <ul>
            <li v-for="link in section.links" :key="link.text">
              <a href="link.href">{{ link.text }}</a>
            </li>
          </ul>
        </section>
      </div>
      <!-- <img src="./../assets/img/dc-logo-bg.png" alt="logo dc" /> -->
    </div>
  </footer>
</template>

<script>
export default {
  name: "AppFooter",
  data() {
    return {
      sections: [
        {
          title: "DC Comics",
          links: [
            {
              href: "#",
              text: "Characters",
            },
            {
              href: "#",
              text: "Comics",
            },
            {
              href: "#",
              text: "Movies",
            },
            {
              href: "#",
              text: "TV",
            },
            {
              href: "#",
              text: "Games",
            },
            {
              href: "#",
              text: "Videos",
            },
            {
              href: "#",
              text: "News",
            },
          ],
        },
        {
          title: "Shop",
          links: [
            {
              href: "#",
              text: "Shop DC",
            },
            {
              href: "#",
              text: "Shop DC Colletibles",
            },
          ],
        },
        {
          title: "DC",
          links: [
            {
              href: "#",
              text: "Term of use",
            },
            {
              href: "#",
              text: "Privacy policy (New)",
            },
            {
              href: "#",
              text: "Ad Choices",
            },
            {
              href: "#",
              text: "Advertising",
            },
            {
              href: "#",
              text: "Jobs",
            },
            {
              href: "#",
              text: "Subscriptions",
            },
            {
              href: "#",
              text: "Talent Workshops",
            },
            {
              href: "#",
              text: "CPSC Certifications",
            },
            {
              href: "#",
              text: "Ratings",
            },
            {
              href: "#",
              text: "Shop Help",
            },
            {
              href: "#",
              text: "Contact Us",
            },
          ],
        },
        {
          title: "Sites",
          links: [
            {
              href: "#",
              text: "DC",
            },
            {
              href: "#",
              text: "MAD Magazine",
            },
            {
              href: "#",
              text: "DC Kids",
            },
            {
              href: "#",
              text: "DC Universe",
            },
            {
              href: "#",
              text: "DC Power Visa",
            },
          ],
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
footer {
  background-image: url("./../assets/img/footer-bg.jpg");
  padding: 1em 0;
}
#links {
  height: 420px;
  display: flex;
  flex-flow: column wrap;
  gap: 1.5em;
  section {
    h1 {
      color: white;
      margin-bottom: 0.5em;
      text-transform: uppercase;
    }
    ul {
      list-style: none;
      li {
        line-height: 1.5em;
      }
      a {
        text-decoration: none;
        color: #5a6161ff;
      }
    }
  }
}
</style>
