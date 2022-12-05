<template>
  <img alt="Vue logo" src="./assets/logo.png" />
  <HelloWorld msg="Hello Vue 3 + TypeScript + Vite" />
  {{ $t /* $t(key: "hello"): void */ }}
  <!-- test section begin -->
  <cw title="bg-info">
    <test-volar
      :data="[{
        full: false,
        nameWidth: 120,
        name: 'Name',
        copy: undefined,
        download: undefined,
        password: undefined,
        value: 'value!!!',
        url: 'a url',
        show: true
      }, {
        full: true,
        nameWidth: undefined,
        name: 'Name2 with full width',
        copy: true,
        download: undefined,
        password: undefined,
        value: 'value2!!!',
        url: 'a url',
        show: true
      }]"
    ></test-volar>
  </cw>
  <!-- test section end -->
</template>

<script lang="ts" setup>
import HelloWorld from './components/HelloWorld.vue'
import TestVolar from './components/TestVolar.vue'
import cw from './components/componentWrapper.vue'
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>

<i18n lang="json">
{
  "en": {
    "hello": "hello world!"
  },
  "ja": {
    "hello": "こんにちは、世界！"
  }
}
</i18n>
