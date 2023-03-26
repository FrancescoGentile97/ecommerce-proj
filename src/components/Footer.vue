<template>
    <footer class="mt-5">
        <!-- newsletter sezione -->
        <section class="my-secondary pb-4 pt-2">
            <div class="container w-50">
                <div class="d-flex flex-column">
                    <h4 class="text-center">Iscriviti alla nostra NewsLetter</h4>
                    <p class="text-center">Lorem ipsum dolor sit amet consectetur adipisicing elit. Amet deserunt minus
                        dolores eum neque est, in
                        fugit blanditiis dicta nulla omnis ab id corporis possimus laboriosam et dignissimos quae deleniti?
                    </p>
                    <div class="d-flex justify-content-center">
                        <label for="" class="form-label"></label>
                        <input type="text" placeholder="Inserisci l'email" class="form-control w-50">
                        <span><i class="fa-regular fa-envelope fs-1 ps-2"></i></span>
                    </div>
                </div>
            </div>
        </section>
        <!-- fine sezione newsletter -->
        <!-- sezione credits -->
        <section class="credits mt-5">
            <div class="container">
                <div class="row text-center">
                    <div class="col-3">
                        <h5>Project Idea</h5>
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Sint non aliquid repellat, beatae natus
                            eius tempora quas, porro facilis.</p>
                        <a href="">Guides</a>
                        <a href="">Term of Use</a>
                        <a href="">Privacy and Policy</a>
                        <i class="fa-regular fa-copyright fs-6"></i>2022-2023
                    </div>
                    <div class="col-3">
                        <h5>Aiuto</h5>
                        <ul class="pt-2">
                            <li class="list-group-item pt-2" v-for="HelpLink in HelpLinks" :key="HelpLink.name">
                                <a href="">
                                    {{ HelpLink.name }}
                                </a>
                            </li>
                        </ul>
                    </div>
                    <div class="col-3">
                        <h5>Chi Siamo</h5>
                        <ul class="pt-2">
                            <li class="list-group-item pt-2" v-for="AboutLink in AboutLinks" :key="AboutLink.name">
                                <a href="">
                                    {{ AboutLink.name }}
                                </a>
                            </li>
                        </ul>
                    </div>
                    <div class="col-3">     
                            <i class="fa-brands fa-instagram pe-1"></i>
                            <i class="fa-brands fa-facebook pe-1"></i>
                            <i class="fa-brands fa-twitter pe-1"></i>
                            <i class="fa-brands fa-linkedin"></i>
                        <h6 class="pt-3">Metodi di pagamento:</h6>
                        <i class="fa-brands fa-cc-paypal pt-4 pe-2"></i>
                        <i class="fa-brands fa-cc-visa"></i>
                    </div>
                </div>
            </div>
        </section>
        <!-- fine sezione credits -->


    </footer>
</template>

<script>
import { store } from '../store';
export default {
    data() {
        return {
            store,
            AboutLinks: [
                {
                    name: "Carriera"
                },
                {
                    name: "Sostenibilità"
                },
                {
                    name: "Servizi"
                },
                {
                    name: "Lavora con noi"
                },
            ],
            HelpLinks: [
                {
                    name: "Stato Ordine",
                },
                {
                    name: "Spedizione e Ritiro",
                },
                {
                    name: "Metodi di Pagamento",
                },
                {
                    name: "Contattaci",
                },
            ],
        }
    }
}

</script>

<style></style>