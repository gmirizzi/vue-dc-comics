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
      <img src="./../assets/img/dc-logo-bg.png" alt="logo dc" />
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
              text: "Collectibles",
            },
            {
              href: "#",
              text: "Videos",
            },
            {
              href: "#",
              text: "Fans",
            },
            {
              href: "#",
              text: "News",
            },
            {
              href: "#",
              text: "Shop",
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
              text: "Collectibles",
            },
            {
              href: "#",
              text: "Videos",
            },
            {
              href: "#",
              text: "Fans",
            },
            {
              href: "#",
              text: "News",
            },
            {
              href: "#",
              text: "Shop",
            },
          ],
        },
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
              text: "Collectibles",
            },
            {
              href: "#",
              text: "Videos",
            },
            {
              href: "#",
              text: "Fans",
            },
            {
              href: "#",
              text: "News",
            },
            {
              href: "#",
              text: "Shop",
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
}
#links {
  width: 30%;
  section {
    ul {
      list-style: none;
    }
  }
}
img {
  width: 70%;
  padding: 0 3em;
}
</style>
