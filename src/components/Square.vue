<template>
  <div class="square">
    <span v-if="value !== ''">
      {{value}}
    </span>
  </div>


</template>

<script>

export default {
  
  name: 'Square',
  props: {
    value: String,
  },
}

</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  .cell {
    width: 64px;
    height: 64px;
    border: 4px;

    display: flex;
    align-items: center;
    justify-content: center;
  }
</style>
