<template>
  <div id="app" class="main-layout">
    <app-header />
    <hero />
    <box />
    <description />
    <starter />
    <app-footer />
  </div>
</template>

<script>
import appHeader from './cmps/app-header'
import hero from './cmps/hero'
import box from './cmps/box'
import description from './cmps/description'
import starter from './cmps/starter'
import appFooter from './cmps/app-footer'

export default {
  name: "app-vue",
  data() {
    return {

    }
  },
  computed: {

  },
  components: {
    appHeader,
    hero,
    box,
    description,
    starter,
    appFooter
  },
};
</script>
