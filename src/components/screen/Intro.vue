<template>
  <div class="intro">
    {{ msg }}
  </div>
</template>

<script lang='ts'>
import Vue from 'vue';

export default Vue.extend({
  name: 'Intro',
  data() {
    return {
      msg: 'intro',
    };
  },
});
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="postcss" scoped>
:root {
  --fontSize: 1em;
}

@custom-media --desktop (width > 768px);
.intro {
  margin: 10px;

  display: grid;
  justify-items: start;
}

</style>
