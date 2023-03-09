<template>
    <section style="width:1080px">
        <div class="container">
            <!-- link del catalogo -->
            <div class="my-primary">
                <h3>Scarpe Uomo</h3>
                <a href="">Home</a>
                <a href="">Catalogo</a>
                <a href="">Uomo</a>
            </div>
            <!-- fine link catalogo -->




            <!-- new:1 section -->
            <div class="d-flex">
                <div class="col sm-6">
                    <div class="card w-100  my-primary">
                        <div class="card-body">
                            <div class="d-flex">
                                <div class="flex-column">
                                    <h5 class="card-title">Card title</h5>
                                    <p class="card-text">With supporting text below as a natural lead-in to additional
                                        content.
                                    </p>
                                    <a href="#" class="btn btn-primary">Button</a>
                                </div>
                                <img src="https://picsum.photos/200" alt="">
                            </div>
                        </div>
                    </div>
                </div>
                <!-- fine new:1 -->

                <!-- new:2 -->
                <div class="col sm-6">
                    <div class="card w-100 my-secondary">
                        <div class="card-body">
                            <div class="d-flex">
                                <div class="flex-column">
                                    <h5 class="card-title">Card title</h5>
                                    <p class="card-text">With supporting text below as a natural lead-in to additional
                                        content.
                                    </p>
                                    <a href="#" class="btn btn-primary">Button</a>
                                </div>
                                <img src="https://picsum.photos/200" alt="">
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <!-- fine new:2 -->

        <!-- toolbar -->
        <div class="row">
            <div class="col">1</div>
            <div class="col">2</div>
            <div class="col">3</div>
            <div class="col">4</div>
        </div>
        <!-- fine tooblar -->

        <!-- sidebar categories... -->
        <div class="d-flex flex-column">

            <!-- lista delle categorie -->
            <ol class="list-group list-group-numbered">
                <li class="list-group-item d-flex justify-content-between align-items-start">
                    <div class="ms-2 me-auto">
                        <div class="fw-bold">
                            <h4>CATEGORIES</h4>
                        </div>
                    </div>
                </li>
                <li class="list-group-item d-flex justify-content-between align-items-start">
                    <div class="ms-2 me-auto">
                        <div class="fw-bold">Subheading</div>
                        Content for list item
                    </div>
                    <span class="badge bg-primary rounded-pill">14</span>
                </li>
                <li class="list-group-item d-flex justify-content-between align-items-start">
                    <div class="ms-2 me-auto">
                        <div class="fw-bold">Subheading</div>
                        Content for list item
                    </div>
                    <span class="badge bg-primary rounded-pill">14</span>
                </li>
            </ol>
        </div>
        <!-- fine lista categorie -->

        <!-- price list -->
        <ol class="list-group list-group-numbered">
            <li class="list-group-item d-flex justify-content-between align-items-start">
                <div class="ms-2 me-auto">
                    <div class="fw-bold">
                        <h4>PRICE</h4>
                    </div>
                </div>
            </li>
            <li class="list-group-item d-flex justify-content-between align-items-start">
                <div class="ms-2 me-auto">
                    <div class="fw-bold">Subheading</div>
                    Content for list item
                </div>
                <span class="badge bg-primary rounded-pill">14</span>
            </li>
            <li class="list-group-item d-flex justify-content-between align-items-start">
                <div class="ms-2 me-auto">
                    <div class="fw-bold">Subheading</div>
                    Content for list item
                </div>
                <span class="badge bg-primary rounded-pill">14</span>
            </li>
        </ol>
        <!-- fine price list -->


        <!-- fine sidebar -->






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
a {
    text-decoration: none;
    padding-right: 0.5rem;
}

.my-primary {
    background-color: orange;
}

.my-secondary {
    background-color: grey;
}

.card-fix {
    padding-left: 0 !important;
    padding-right: 0 !important;
}
</style>