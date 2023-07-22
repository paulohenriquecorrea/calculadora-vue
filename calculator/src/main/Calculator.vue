<template>
  <div class="calculator">
    <Button />
  </div>
</template>

<script>
import Button from "../componentes/Button";
export default {
  name: "DefaultCalculator",
  components: { Button },
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