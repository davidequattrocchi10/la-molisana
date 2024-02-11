<script >
import AppLogo from './AppLogo.vue';

export default {
    name: "AppHeader",
    components: {
        AppLogo
    }
}

</script>

<template>
    <header>
        <AppLogo></AppLogo>
        <nav>
            <ul class="main_menu">
                <li><a href="#">Home</a></li>
                <li><a href="#" class="active">Prodotti</a></li>
                <li><a href="#">Chi siamo</a></li>
                <li><a href="#">Contatti</a></li>
            </ul>
        </nav>
    </header>
</template>

<style scoped>
header {
    text-align: center;
    background-color: var(--moli-light);

    & .main_menu {
        list-style: none;
        display: flex;
        justify-content: center;

        & li {
            margin: 2rem;
        }

        & a {
            text-decoration: none;
            padding: 1rem;
            color: var(--moli-dark);
            font-weight: 600;
        }

        & a.active {
            background-color: var(--moli-lightblue);
        }
    }
}
</style>