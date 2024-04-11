<script >

  import AppHeader from './components/AppHeader.vue';
  import AppContentCentral from './components/AppContentCentral.vue';
  import AppCardSection from './components/AppCardSection.vue';
  import AppFooterLink from './components/AppFooterLink.vue';
  import AppFooterInfo from './components/AppFooterInfo.vue';

  export default {
    components: {
      AppHeader,
      AppContentCentral,
      AppCardSection,
      AppFooterLink,
      AppFooterInfo
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
<AppFooterInfo></AppFooterInfo>
</footer>
</template>

<style lang="scss">
  @use './style/generic' as *;
</style>
