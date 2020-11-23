<template>
  <li>
    <base-card>
      <header>
        <h3>{{ title }}</h3>
        <base-button mode="flat">Delete</base-button>
      </header>
      <p></p>
      <nav>
        <a :href="link">{{ description }}</a>
      </nav>
    </base-card>
  </li>
</template>

<script>
export default {
  props: ['title', 'description', 'link'],
};
</script>

<style scoped>
li {
  margin: auto;
  max-width: 40rem;
}
nav a {
  color: orange;
  text-decoration: none;
}
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
</style>