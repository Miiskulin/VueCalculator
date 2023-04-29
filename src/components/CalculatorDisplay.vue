<template>
  <div class="CalculatorDisplay">
    {{ value }}
  </div>
</template>

<script>
export default {
  props: ['value']
}
</script>

<style>
 .CalculatorDisplay{
  grid-column: span 4;
  background-color: #0004;

  display: flex;
  justify-content: flex-end;
  align-items: center;
  padding: 20px;
  font-size: 2.2em;
  overflow: hidden;

 }
</style>