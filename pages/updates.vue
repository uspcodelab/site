<template>
  <div class="page">
    <the-navbar/>
    <b-container fluid>
      <main>
        <MonthlyUpdates />
      </main>
      <the-footer/>
    </b-container>
  </div>
</template>

<script>
import TheNavbar from "~/components/TheNavbar.vue";
import TheFooter from "~/components/TheFooter.vue";
import MonthlyUpdates from "~/components/MonthlyUpdates.vue";

export default {
  components: {
    TheNavbar,
    TheFooter,
    MonthlyUpdates
  }
};
</script>

<style lang="scss">
html {
  font-size: 14px;
}

.page {
  padding-top: 4rem;
}

@include media-breakpoint-up(lg) {
  html {
    font-size: 16px;
  }
}

@include media-breakpoint-up(xl) {
  html {
    font-size: 1.5vmax;
  }
}
</style>
