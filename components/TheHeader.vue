<template>
  <div class="header">
    <div class="top">
      <div class="logo-container">
        <nuxt-picture
          src="/images/logo.png"
          fit="contain"
          width="100"
          height="100"
        />
        <h1 class="logoTitle">SwoonMe</h1>
      </div>
      <SearchBar />
      <div class="header-button-container">
        <HeaderButtons iconName="person" label="Profil" />
        <HeaderButtons iconName="shopping_basket" label="Mon panier" />
      </div>
    </div>
    <!-- <div class="bottom" id="app">
      <HeaderButtonsMenu
        v-for="item in objectItems"
        :key="item"
        :button="item"
      />
    </div> -->
  </div>
</template>

<script>
import SearchBar from "./Inputs/SearchBar.vue";
import HeaderButtons from "./Buttons/HeaderButtons.vue";
import HeaderButtonsMenu from "./Buttons/HeaderButtonsMenu.vue";
export default {
  head() {
    return {
      bodyAttrs: {
        class: "reset-body",
      },
    };
  },
  components: { SearchBar, HeaderButtons, HeaderButtonsMenu },
};
</script>
<style src="@/assets/header.css" />

<style>
.reset-body {
  margin: 0;
}
</style>
