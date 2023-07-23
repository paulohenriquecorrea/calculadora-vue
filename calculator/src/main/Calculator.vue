<template>
  <div class="calculator">
    <Display :value="displayValue" />
    <Button />
  </div>
</template>

<script>
import Button from "../componentes/Button";
import Display from "../componentes/Display";
export default {
  name: "DefaultCalculator",
  components: { Button, Display },
  data: function () {
    return {
      displayValue: "0",
    };
  },
};
</script>

<style scoped>
.calculator {
  height: 320px;
  width: 235px;
  border-radius: 5px;
  overflow: hidden;

  display: grid;
  grid-template-columns: repeat(4, 25%);
  grid-template-rows: 1fr 48px 48px 48px 48px 48px;
}
</style>