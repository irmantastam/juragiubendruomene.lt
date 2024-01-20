<script setup>
import illustration from "./Illustration.vue";

defineProps({
  msg: String,
});
</script>

<template>
  <img
    class="main-image"
    width="400"
    height="300"
    src="../assets/juragiu_bendruomene.webp"
    alt="Juragių bendruomenės centras"
  />

  <h1>{{ msg }}</h1>
  <p class="slogan">Būkime kartu!</p>

  <div class="card">
    <h2>Mūsų adresas:</h2>
    <p class="address">Girininkų g. 6, Juragiai, LT-53286 Kauno r.</p>

    <a
      href="https://maps.app.goo.gl/r9A1W6LbUiGoJLtW8"
      target="_blank"
      rel="noopener noreferrer"
    >
      Žr. žemėlapyje 🌍
    </a>
  </div>

  <div class="card">
    <a
      href="https://www.facebook.com/profile.php?id=100067655868254"
      target="_blank"
      rel="noopener noreferrer"
    >
      Sekite mus Facebook! ⓕ
    </a>
  </div>

  <illustration />

  <p class="link">juragiubendruomene.lt 2024</p>
</template>

<style scoped>
.main-image {
  border-radius: 0.4em;
  max-width: 100%;
  border: 0.1em solid rgb(207 217 224/1);
  box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1),
    0 4px 6px -4px rgba(0, 0, 0, 0.1);
}

.slogan {
  margin: 0;
  margin-top: -1em;
}

h2 {
  margin-top: 0;
}

.address {
  margin-top: -0.4em;
}

.link {
  font-size: 0.8em;
  font-weight: 500;
}
</style>
