<template>
  <div id="app">
    <b-container class="shadow-lg px-0 overflow-hidden">
      <b-navbar toggleable="lg" type="light" variant="white" :sticky="stickable">
        <b-navbar-toggle class="border-0" target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav>
            <b-nav-item href="/">ACCUEIL</b-nav-item>
            <b-nav-item href="projets.html">PROJETS</b-nav-item>
            <b-nav-item href="portfolio.html">PORTFOLIO</b-nav-item>
            <b-nav-item href="#" active>CONTACT</b-nav-item>
          </b-navbar-nav>

          <!-- <b-navbar-nav class="ml-auto">
            <b-nav-item href="#" class="darkmode-icon"><img src="/dark-mode.svg" width="20px" alt="Darkmode Switcher"></b-nav-item>
          </b-navbar-nav> -->
        </b-collapse>
      </b-navbar>
      <b-row>
        <GradientBlueBanner page="Mes réseaux"/>
      </b-row>
      <b-row class="mx-0">
        <b-col md="6" lg="3" class="px-0 d-flex justify-content-center">
          <SocialMediaItem icon="twitter" name="elias54_" url="https://twitter.com/elias54_" colorCode="#1DA1F2"/>
        </b-col>
        <b-col md="6" lg="3" class="px-0 d-flex justify-content-center">
          <SocialMediaItem icon="facebook-f" name="Eliferd" url="https://www.facebook.com/elif3rd" colorCode="#1778F2"/>
        </b-col>
        <b-col md="6" lg="3" class="px-0 d-flex justify-content-center">
          <SocialMediaItem icon="instagram" name="eliferd_" url="https://www.instagram.com/eliferd_/" colorCode="#DD2A7B"/>
        </b-col>
        <b-col md="6" lg="3" class="px-0 d-flex justify-content-center">
          <SocialMediaItem icon="youtube" name="Eliferd" url="https://www.youtube.com/user/eliaas54" colorCode="#FF0000"/>
        </b-col>
      </b-row>
      <b-row class="mx-0">
        <b-col md="6" lg="3" class="px-0 d-flex justify-content-center">
          <SocialMediaItem icon="steam-square" name="Eliferd" url="http://steamcommunity.com/id/elias54700" colorCode="#2A475E"/>
        </b-col>
        <b-col md="6" lg="3" class="px-0 d-flex justify-content-center">
          <SocialMediaItem icon="github" name="eliferd" url="https://github.com/eliferd" colorCode="#211F1F"/>
        </b-col>
        <b-col md="6" lg="3" class="px-0 d-flex justify-content-center">
          <SocialMediaItem icon="vimeo-v" name="eliferd" url="https://vimeo.com/eliferd" colorCode="#19B7EA"/>
        </b-col>
        <b-col md="6" lg="3" class="px-0 d-flex justify-content-center">
          <SocialMediaItem icon="dribbble" name="eliferd" url="https://dribbble.com/eliferd" colorCode="#EA4C89"/>
        </b-col>
      </b-row>
      <b-row>
        <b-col md="6" lg="3" class="px-0 d-flex justify-content-center">
          <SocialMediaItem icon="twitch" name="elias54_" url="https://www.twitch.tv/elias54_" colorCode="#6441A4"/>
        </b-col>
      </b-row>
      <hr>
      <b-row>
        <b-col cols="12" class="mb-3 text-center">
          Eliferd © 2021 Tous droits réservés.
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<style src="./style.css"></style>
<script>
import GradientBlueBanner from '../components/GradientBlueBanner.vue'
import SocialMediaItem from '../components/SocialMediaItem.vue'

export default {
  name: 'Projets',
  components: {
    GradientBlueBanner,
    SocialMediaItem
  },
  props: {
    sticky: {
      type: Boolean
    }
  },
  computed: {
    stickable: function () {
      return true
    }
  }
}
</script>
