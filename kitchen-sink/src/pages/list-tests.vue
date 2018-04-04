<template>
  <f7-page>
    <f7-navbar title="List tests"/>
    <f7-list>
      <f7-list-item v-for="item in list">{{ item }}</f7-list-item>
    </f7-list>

    <f7-button fill @click="list.push('li')">Text</f7-button>
  </f7-page>
</template>

<script>
  import { f7Page, f7Navbar, f7List, f7ListItem, f7Button } from 'framework7-vue';

  export default {
    components: {
      f7Page,
      f7Navbar,
      f7List,
      f7ListItem,
      f7Button,
    },

    data: () => ({
      list: [],
    }),
  };
</script>
