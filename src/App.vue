<template>
  <div id="app">
    <!-- <PictoBtn :icon="icon" :color="color" /> -->
    <ExecutiveSummary />
  </div>
</template>

<script>
import PictoBtn from './components/ExecutiveSummary/PictoBtn';
import ExecutiveSummary from './components/ExecutiveSummary';

export default {
  name: 'App',
  components: {
    PictoBtn,
    ExecutiveSummary,
  },
  data() {
    return {
      icon: 'finger',
      color: 'bg-pink-300',
    };
  },
};
</script>

<style>
body {
  background: #363636;
  padding: 50px;
}
</style>
