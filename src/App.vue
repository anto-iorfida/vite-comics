<script >

  import AppHeader from './components/AppHeader.vue';
  import AppContentCentral from './components/AppContentCentral.vue';
  import AppCardSection from './components/AppCardSection.vue';

  export default {
    components: {
      AppHeader,
      AppContentCentral,
      AppCardSection
    }
  }
  
</script>

<template>
<AppHeader></AppHeader>

<main>
<AppContentCentral></AppContentCentral>
<AppCardSection></AppCardSection>
</main>
</template>

<style lang="scss">
  @use './style/generic' as *;
</style>
