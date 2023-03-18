<template>
    <section class="temp-fix">
    <nav class="navbar navbar-expand-lg fixed-top bg-light navbar-light">
        <div class="container d-flex">
            <div>
                <ul class="navbar-nav ms-auto align-items-center">
                    <li class="nav-item">
                        <a class="nav-item mx-2" href="#!"><i class="fa-solid fa-magnifying-glass"></i></a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-item mx-2" href="#!"><i class="fa-solid fa-bars me-2"></i>Categoria</a>
                    </li>
                </ul>
            </div>
            <div>
                <h5><a href="#!">Progetto E-Commerce</a></h5>
            </div>
            <div>
                <ul class="navbar-nav ms-auto align-items-center">
                <li class="nav-item">
                        <a class="nav-link mx-2" href="#!"><i class="fa-solid fa-user"></i></a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link mx-2" href="#!"><i class="fa-solid fa-heart"></i></a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link mx-2" href="#!"><i class="fa-solid fa-cart-shopping"></i></a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-item mx-2" href="#!"><i class="fa-solid fa-magnifying-glass"></i></a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
</section>
</template>

<script>
import { store } from '../store';
export default {
    data() {
        return {
            store,
        }
    }
}


</script>

<style scoped>
.my-index{
    z-index: 9999;
}
.temp-fix{
    margin-bottom: 15.5rem;
}
</style>