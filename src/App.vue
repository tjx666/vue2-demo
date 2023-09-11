<script lang="ts" setup>
import { ref } from 'vue';

const count = ref(0);

function increase() {
    count.value++;
}
</script>

<template>
    <div class="counter">
        <h2 class="title">{{ count }}</h2>
        <button class="plus" @click="increase">+</button>
    </div>
</template>

<style lang="css" scoped>
body {
    width: 100vw;
    height: 100vh;
}

.counter {
    width: 200px;
    margin: 60px auto 0;
    display: flex;
    flex-direction: column;
    align-items: center;

    .plus:active {
        background-color: orange;
    }
}
</style>
