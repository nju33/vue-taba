<template>
  <div ref="taba"></div>
</template>

<script>
import Taba from 'taba';

export default {
  props: {
    styleObj: {
      type: Object,
      default: () => ({})
    },
    data: {
      type: Object,
      required: true
    }
  },
  mounted() {
    console.log(this);
    new Taba({
      target: this.$refs.taba,
      data: {
        style: this.styleObj,
        data: this.data,
      }
    });
  }
}
</script>
