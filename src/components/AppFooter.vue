<script>
import AppLogo from './AppLogo.vue';

export default {
    name: 'AppFooter',
    components: { AppLogo }
}

</script>
<template>
    <footer>
        <div class="container">
            <div class="row">
                <div class="col-12 col-md-6  col-lg-4">
                    <AppLogo></AppLogo>
                </div>
                <div class="col-12 col-md-6  col-lg-4">
                    <h3>PASTIFICIO</h3>
                    <ul class="list-unstyled">
                        <li><a href="">Il Pastificio</a></li>
                        <li><a href="">Grano</a></li>
                        <li><a href="">Filiera</a></li>
                        <li><a href="">100 anni di pasta</a></li>
                        <li><a href="">Sartoria della pasta</a></li>
                    </ul>
                </div>
                <div class="col-12 col-md-6  col-lg-4">
                    <h3>PRODOTTI</h3>
                    <ul class="list-unstyled">
                        <li><a href="">Le classiche</a></li>
                        <li><a href="">Le integrali</a></li>
                        <li><a href="">Le speciali</a></li>
                        <li><a href="">Le Biologiche</a></li>
                        <li><a href="">Le Gluten-free</a></li>
                    </ul>
                </div>
            </div>
        </div>
    </footer>
</template>
<style scoped>
footer {
    padding-top: 2rem;
    min-height: 400px;
    background-color: var(--moli-light);
    background-image: url(/img/footer-montagne-bottom.jpg);
    background-position: bottom;
    background-repeat: no-repeat;

    & h3 {
        color: var(--moli-darkblue);
        margin-bottom: 1rem;
    }

    & ul.list-unstyled {
        & a {
            text-decoration: none;
            color: var(--moli-dark);
        }
    }
}
</style>