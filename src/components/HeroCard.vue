<template>
  <section class="hero-card">
    <h2>{{ hero.name }}</h2>
    <img :src="require(`../assets/${hero.image}`)" :alt="hero.name" />
    <p>{{ hero.description }}</p>
  </section>
</template>

<script>
export default {
  name: "HeroCard",
  props: {
    hero: Object,
  },
};
</script>

<style scoped>
.hero-card {
  margin-bottom: 3em;
}
.hero-card img {
  max-width: 100%;
  height: auto;
  border-radius: 8px;
  box-shadow: 0 2px 6px rgba(0,0,0,0.2);
  margin: 0.5em 0 1em 0;
}
</style>
