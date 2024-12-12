<template>
    <div class="header">
        <h1>{{ title }}</h1>
        <button @click="handleClick">Click Me</button>
    </div>
</template>

<script>
    export default {
        props: ['title'],
        methods: {
            handleClick() {
                alert('Button clicked!');
            }
        }
    }
</script>

<style>
    .header {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 10px;
        background-color: #f8f9fa;
        border-bottom: 1px solid #dee2e6;
    }
    button {
        padding: 5px 10px;
        border: none;
        background-color: #007bff;
        color: white;
        cursor: pointer;
    }
</style>
