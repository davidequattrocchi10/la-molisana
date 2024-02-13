<script>
export default {
    name: 'ProductCard',
    props: {
        product: Object
    }
}
</script>

<template>
    <div class="product">
        <img v-bind:src="product.src" alt="">
        <h3> {{ product.titolo }}</h3>
    </div>
</template>


<style scoped>
.product {
    background-color: var(--moli-light);
    height: 100%;
    border-radius: 1rem;

    &:hover {
        filter: drop-shadow(0 0 10px var(--moli-darkblue));
    }

    & img {
        border-top-right-radius: 1rem;
        border-top-left-radius: 1rem;

    }

    & h3 {
        padding: 1rem;
    }


}
</style>