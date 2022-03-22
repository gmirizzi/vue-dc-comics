<template>
  <header>
    <nav>
      <ul>
        <li v-for="link in links" :key="link.text">
          <a href="link.href">{{ link.text }}</a>
        </li>
      </ul>
    </nav>
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
ul {
  list-style: none;
  li {
    display: inline-block;
    margin: 1em;
    a {
      display: inline-block;
      text-decoration: none;
    }
  }
}
</style>
