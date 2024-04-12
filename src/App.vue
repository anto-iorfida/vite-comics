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
  <!-- header with menu and logo -->
<AppHeader></AppHeader>

<main>
<!-- Section with card cinema   -->
<AppContentCentral></AppContentCentral>
<!-- section with icon and information-->
<AppCardSection></AppCardSection>
</main>

<footer>
<!-- section  whit link-->
<AppFooterLink></AppFooterLink>
<!-- section whit info and icon social -->
<AppFooterInfo></AppFooterInfo>
</footer>
</template>

<style lang="scss">
  @use './style/generic' as *;
</style>
