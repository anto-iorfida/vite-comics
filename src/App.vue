<script >

  import AppHeader from './components/AppHeader.vue';
  import AppContentCentral from './components/AppContentCentral.vue';
  import AppCardSection from './components/AppCardSection.vue';
  import AppFooterLink from './components/AppFooterLink.vue';

  export default {
    components: {
      AppHeader,
      AppContentCentral,
      AppCardSection,
      AppFooterLink
    }
  }
  
</script>

<template>
<AppHeader></AppHeader>

<main>
<AppContentCentral></AppContentCentral>
<AppCardSection></AppCardSection>
</main>

<footer>
<AppFooterLink></AppFooterLink>
</footer>
</template>

<style lang="scss">
  @use './style/generic' as *;
</style>
