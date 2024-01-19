<script setup>
import { ref } from "vue";

defineProps({
  msg: String,
});
</script>

<template>
  <img
    class="main-image"
    width="360"
    src="../assets/juragiu_bendruomene.webp"
  />

  <h1>{{ msg }}</h1>

  <h3>Adresas:</h3>

  <p>Girininkų g. 6, Juragiai, LT-53286 Kauno r.</p>

  <p>
    <a
      href="https://maps.app.goo.gl/r9A1W6LbUiGoJLtW8"
      target="_blank"
      rel="noopener noreferrer"
    >
      Žr. žemėlapyje 🌍
    </a>
  </p>

  <p class="card">
    <a
      href="https://www.facebook.com/profile.php?id=100067655868254"
      target="_blank"
      rel="noopener noreferrer"
    >
      Aplankykite mus Facebook! ⓕ
    </a>
  </p>
</template>

<style scoped>
.main-image {
  border-radius: 100%;
  aspect-ratio: 1;
}
</style>
