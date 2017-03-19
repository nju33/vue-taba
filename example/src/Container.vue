<template lang="html">
  <Taba :styleObj="style" :data="data"/>
</template>

<script>
import Taba from 'components/Taba';

export default {
  components: {
    Taba
  },
  data() {
    return {
      style: {
        height: '50vh'
      },
      data: {
        header: {
          data: ['testtest', 'testtest', 'testtest', 'testtest', 'testtest', 'testtest', 'testtest'],
          fixed: true
        },
        body: {
          data: [
            ['testtest', 'testtest', 'testtest', 'testtest', 'testtest', 'testtest', 'testtest'],
            ['testtest', 'testtest', 'testtest', 'testtest', 'testtest', 'testtest', 'testtest'],
            ['testtest', 'testtest', 'testtest', 'testtest', 'testtest', 'testtest', 'testtest'],
            ['testtest', 'testtest', 'testtest', 'testtest', 'testtest', 'testtest', 'testtest'],
            ['testtest', 'testtest', 'testtest', 'testtest', 'testtest', 'testtest', 'testtest'],
            ['testtest', 'testtest', 'testtest', 'testtest', 'testtest', 'testtest', 'testtest'],
            ['testtest', 'testtest', 'testtest', 'testtest', 'testtest', 'testtest', 'testtest'],
            ['testtest', 'testtest', 'testtest', 'testtest', 'testtest', 'testtest', 'testtest'],
            ['testtest', 'testtest', 'testtest', 'testtest', 'testtest', 'testtest', 'testtest']
          ],
          zip: true,
          fixed: 1
        },
        footer: {
          data: ['testtest', 'testtest', 'testtest', 'testtest', 'testtest', 'testtest', 'testtest'],
          fixed: true
        },
      }
    };
  },
}
</script>

<style>
body {
  margin: 0;
}
</style>

<style scoped>
.p {
  position: absolute;
  bottom: 50%;
  right: 50%;
  transform: translate(50%, 50%);
  background: #ccc;
  margin: 1em;
  height: 2em;
  width: 30%;
}
</style>
