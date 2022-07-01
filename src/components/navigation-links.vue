<template>
  <nav class="navigation-links-nav" v-bind:class="rootClassName">
    <router-link to="/about" class="navigation-links-navlink">
      {{ text }}
    </router-link>
    <span class="navigation-links-text">{{ text1 }}</span>
    <span class="navigation-links-text1">{{ text2 }}</span>
    <span class="navigation-links-text2">{{ text3 }}</span>
    <span class="navigation-links-text3">{{ text4 }}</span>
  </nav>
</template>

<script>
export default {
  name: 'NavigationLinks',
  props: {
    text: {
      type: String,
      default: 'About',
    },
    text3: {
      type: String,
      default: 'Team',
    },
    text4: {
      type: String,
      default: 'Blog',
    },
    text1: {
      type: String,
      default: 'Features',
    },
    rootClassName: String,
    text2: {
      type: String,
      default: 'Pricing',
    },
  },
}
</script>

<style scoped>
.navigation-links-nav {
  flex: 0 0 auto;
  display: flex;
  align-items: center;
  flex-direction: row;
}
.navigation-links-navlink {
  text-decoration: none;
}
.navigation-links-text {
  margin-left: 32px;
}
.navigation-links-text1 {
  margin-left: 32px;
}
.navigation-links-text2 {
  margin-left: 32px;
}
.navigation-links-text3 {
  margin-left: 32px;
}









@media(max-width: 767px) {
  .navigation-links-nav {
    align-items: flex-start;
    flex-direction: column;
  }
  .navigation-links-navlink {
    margin-bottom: var(--dl-space-space-unit);
  }
  .navigation-links-text {
    margin-left: 0;
    margin-bottom: var(--dl-space-space-unit);
  }
  .navigation-links-text1 {
    margin-left: 0;
    margin-bottom: var(--dl-space-space-unit);
  }
  .navigation-links-text2 {
    margin-left: 0;
    margin-bottom: var(--dl-space-space-unit);
  }
  .navigation-links-text3 {
    margin-left: 0;
    margin-bottom: var(--dl-space-space-unit);
  }
}
</style>
