<template>
  <q-page-container>
    <q-header elevated>
      <q-toolbar color="red">
        <q-btn flat dense round icon="menu" @click="$refs.drawer.open()" aria-label="Menu" />
        <q-toolbar-title>
          kd jayakody blog
        </q-toolbar-title>
        <q-btn flat dense round label="Home" @click="goToPage('home')" />
        <q-btn flat dense round label="About" @click="goToPage('about')" />
        <q-btn flat dense round label="Contact" @click="goToPage('contact')" />
      </q-toolbar>
    </q-header>

    <q-page padding>
      <div class="content">
        <h2>Welcome to My Blog</h2>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed quis velit a lectus tincidunt fringilla. Donec in felis eget nunc tempor venenatis. Sed in risus sit amet odio tempor lacinia.
        </p>
        <p>
          Integer nec neque non turpis consequat hendrerit. Suspendisse potenti. Nullam tincidunt vel mi eget suscipit. Vivamus eu quam a purus rutrum tristique.
        </p>
      </div>
    </q-page>
  </q-page-container>
</template>

<script>
export default {
  methods: {
    goToPage(page) {
      this.$router.push({ name: page });
    },
  },
};
</script>

<style scoped>
.content {
  max-width: 800px;
  margin: 0 auto;
  padding: 20px;
}
</style>
