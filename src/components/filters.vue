<template>
    <div class="filters">
        <button>Новинки</button>
        <button>Есть в наличии</button>
        <button>Контрактные</button>
        <button>Эксклюзивные</button>
        <button>Распродажа</button>
    </div>
</template>

<script>
    export default {
        name: 'filters'
    }
</script>

<style scoped>
    .filters {
        display: flex;
        flex-direction: column;
        text-transform: uppercase;
    }
</style>