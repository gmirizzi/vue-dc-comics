<template>
  <header>
    <div class="container">
      <img src="./../assets/img/dc-logo.png" alt="logo dc" />
      <nav>
        <ul>
          <li v-for="link in links" :key="link.text">
            <a href="link.href">{{ link.text }}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "AppHeader",
  data() {
    return {
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
    };
  },
};
</script>

<style scoped lang="scss">
.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  img {
    width: 100px;
    padding: 1em;
  }
  ul {
    list-style: none;
    li {
      display: inline-block;
      margin: 0.5em;
      a {
        font-size: 0.7rem;
        text-transform: uppercase;
        display: inline-block;
        text-decoration: none;
        color: unset;
      }
    }
  }
}
</style>
