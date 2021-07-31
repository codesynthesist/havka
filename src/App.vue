<template>
  <div id="app">
    <Header/>
    <router-view/>
  </div>
</template>

<script lang="ts">
import Header from '@/components/Header.vue';
import { Vue, Component } from 'vue-property-decorator';

@Component({
  components: {
    Header,
  },
})

export default class App extends Vue {

}
</script>
