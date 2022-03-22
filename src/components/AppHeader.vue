<template>
  <header>
    <div class="container">
      <img src="./../assets/img/dc-logo.png" alt="logo dc" />
      <nav>
        <ul>
          <li
            v-for="(link, index) in links"
            :key="link.text"
            :class="{ active: index == activeIndex }"
            @click.stop.prevent="activeIndex = index"
          >
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
      activeIndex: 1,
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
  height: 100px;
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
      margin: 1em;
      a {
        line-height: calc(100px - 1em);
        font-size: 0.7rem;
        text-transform: uppercase;
        display: inline-block;
        text-decoration: none;
        color: unset;
      }
    }
  }
}
.active {
  color: #0282f9ff;
  a {
    border-bottom: 1em solid #0282f9ff;
  }
}
</style>
