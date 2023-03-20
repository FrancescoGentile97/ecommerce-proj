<template>
    <footer class="bg-primary mt-5">
        <!-- newsletter sezione -->
        <div class="container w-50">
            <div class="d-flex flex-column">
                <h4 class="text-center">Iscriviti alla nostra NewsLetter</h4>
                <p class="text-center">Lorem ipsum dolor sit amet consectetur adipisicing elit. Amet deserunt minus
                    dolores eum neque est, in
                    fugit blanditiis dicta nulla omnis ab id corporis possimus laboriosam et dignissimos quae deleniti?
                </p>
                <div class="d-flex justify-content-center">
                    <label for="" class="form-label"></label>
                    <input type="text" placeholder="Inserisci l'email" class="form-control w-50 bg-secondary">
                    <span><i class="fa-regular fa-envelope fs-1 ps-2"></i></span>
                </div>
            </div>
        </div>
        <!-- fine sezione newsletter -->


    </footer>
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

<style></style>