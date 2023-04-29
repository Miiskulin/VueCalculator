<template>
  <div id="app">
    <h1>Calculator</h1>
    <MainCalculator />
  </div>
</template>

<script>
import MainCalculator from "./main/MainCalculator"

export default {
    components: { MainCalculator }
}
</script>

<style>
@font-face{
    font-family: "RobotoMono";
    src: url("./fonts/RobotoMono-VariableFont_wght.ttf");
}

* {
    font-family: "RobotoMono", monospace;
}

body {
    margin: 0;
}

#app {
    display: flex;
    flex-direction: column;
    height: 100vh;
    justify-content: center;
    align-items: center;
    text-align: center;
    color: #FFFAFA;
    background: linear-gradient(90deg, hsla(159, 35%, 45%, 1) 0%, hsla(176, 68%, 12%, 1) 100%);
}
</style>