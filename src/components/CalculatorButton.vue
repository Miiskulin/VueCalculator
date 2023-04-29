<template>
  <button class="CalculatorButton" @click="$emit('onClick', label)" :class="{double, triple, operation}">
    {{ label }}
  </button>
</template>

<script>
export default {
  props:{
    label:{},
    operation: {type: Boolean},
    double: { type: Boolean },
    triple: { type: Boolean }
  }
}
</script>

<style>
 /* /pseudoclasse */
:root{ 
  --bg-button: #EFD6AC;
  --border-button: solid 1px #1F1F1F;
}

.CalculatorButton{
  font-size: 1.4em;
  background-color: var(--bg-button);
  border: none;
  border-right: var(--border-button); /*pq muda os dois border e um só não */
  border-bottom: var(--border-button);
  outline: none;
}

.CalculatorButton:active{
  background-color: #EFD6ACcc;
}

.CalculatorButton.double{
  grid-column:span 2;
}

.CalculatorButton.triple{
  grid-column:span 3;
}

.CalculatorButton.operation{
  background-color:#C44900;
  color: #fff;
}

.CalculatorButton.operation:active{
  background-color: #C44900cc;
}

</style>