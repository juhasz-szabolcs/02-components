<script setup>
    defineProps({
        title: {
            type: String,
            required: true,
            default: 'Default Title'
        }
    });
</script>

<template>
    <nav>
        <ul>
            <li><a href="/">{{ title }}</a></li>
            <li><a href="https://vuejs.org/">Vue.js</a></li>
        </ul>
    </nav>
</template>

<style scoped>
    nav {
        background-color: lightgray;
        padding: 1rem;
    }

    ul {
        display: flex;
        list-style: none;
        padding: 0;
        margin: 0;
    }

    li {
        margin-right: 1rem;
    }

    a {
        text-decoration: none;
        color: #333;
        font-size: 1.2rem;
        padding: 0.5rem 1rem;
    }
</style>