<script setup>
import Description from './components/Description.vue'
import ContactForm from './components/ContactForm.vue'
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="./assets/company.png" width="600" height="600" />
  </header>

  <main>
    <div id="Description">
    <Description />
    </div>
    <div id="ContactForm">
    <ContactForm />
    </div>
  </main>
</template>

<style scoped>
#Description{display:block;}
#ContactForm{display:none;}

header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
