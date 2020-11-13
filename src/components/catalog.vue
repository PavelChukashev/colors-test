<template>
    <div class="catalog">
        <Filters />
        <CatalogItem />
    </div>
</template>

<script>
import CatalogItem from './catalog-item.vue'
import Filters from './filters.vue'

export default {
    name: 'catalog',
    components: {
        CatalogItem,
        Filters,
    }
}
</script>

<style scoped>
    .catalog {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
        align-items: flex-end;
        margin: 0 auto;
    }
    .box {
        padding: 20px;
        border: 2px solid black;
    }
</style>