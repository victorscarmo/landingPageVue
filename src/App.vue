<script setup>
// Styles
import styles from "./App.module.css";

// Components
import Header from "./components/Header/Header.vue";
import Main from "./components/Main/Main.vue";
import Footer from "./components/Footer/Footer.vue";
</script>

<template>
  <div :class="styles.container">
    <Header />
    <Main />
    <Footer />
  </div>
</template>