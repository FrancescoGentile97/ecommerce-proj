<template>
    <section>
        <div class="w-100">
            <!-- link del catalogo -->
            <div class=" text-center my-padding-top pb-5 my-secondary">
                <h3>Scarpe Uomo</h3>
                <a href="">Home</a>
                <a href="">Catalogo</a>
                <a href="">Uomo</a>
            </div>
        </div>
    </section>

    <!-- fine link catalogo -->




    <!-- new section -->
    <div class="container my-negative-mt">
        <div class="row">
            <div class="col-8  card-fix">
                <div class="w-100 my-third">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-4 ps-4">
                                <div class="my-badge">
                                    <p class="text-white my-badge-new">New</p>
                                </div>
                                <h5 class="card-title mt-4 mb-2">Scarpe</h5>
                                <p class="card-text mb-4">Nike Dunk High Halloween</p>
                                <a href="#" class="myButton mt-4">Più Informazioni</a>
                            </div>

                            <div class="col-8">
                                <img src="../assets/dunk-high-halloween-1_2000x.webp" alt="" class="img-fluid img-new-1">
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="col-4 card-fix">
                <div class="w-100  my-primary">
                    <div class="card-body">
                        <div class="row">
                            <div class="col-6 ps-4">
                                <div class="my-badge">
                                    <p class="text-white my-badge-new">New</p>
                                </div>
                                <h5 class="card-title mt-4 mb-2">Giacchetto</h5>
                                <p class="card-text mb-4">Air Jordan Giacchetto</p>
                                <a href="#" class="myButton mt-4">Più Informazioni</a>
                            </div>
                            <div class="col-6">
                                <img src="../assets/jordan-jacket.webp" alt="" class="img-fluid img-new-2">
                            </div>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </div>
    <!-- fine new section -->

    <!-- toolbar -->
    <div class="container">
        <div class="row">
            <div class="my-filter-bar my-border justify-content-between py-4 ">
                Filter
                <div class="border"></div>
                <span><i class="fa-solid fa-rotate"></i></span>

            </div>
            <div class="col d-flex justify-content-between my-border py-4">
                Venduto da:
                <span><i class="fa-solid fa-caret-down"></i></span>
            </div>
            <div class="col d-flex justify-content-between my-border py-4">
                Trovati:12
                <span><i class="fa-solid fa-caret-down"></i></span>
            </div>
            <div class="col d-flex justify-content-between my-border py-4">
                <i class="fa-solid fa-table-cells"></i>
                <i class="fa-solid fa-list"></i>
                Compara:
                <span class="badge bg-primary rounded-pill">3</span>
            </div>
        </div>
    </div>
    <!-- fine tooblar -->

    <!-- sidebar categories... -->
    <div class="container my-p-unset">
        <div class="sidebar">
            <div class="d-flex flex-column">

                <!-- lista delle categorie -->
                <ul class="list-group">
                    <div class="list-group-item d-flex justify-content-between align-items-start">
                        <div class="fw-bold">
                            <h5>CATEGORIES</h5>
                        </div>
                    </div>
                    <li v-for="category in categories" :key="category.title" class="list-group-item d-flex justify-content-between align-items-start">
                        {{ category.title }}
                        <span class="badge bg-primary rounded-pill">
                            {{ category.badge}}
                        </span>
                    </li>
                </ul>
            </div>
            <!-- fine lista categorie -->

            <!-- price range bar -->
            <div id="form-wrapper">
                <form action="/p/quote.php" method="GET">
                    <h4 id="form-title">Seleziona il prezzo</h4>
                    <div id="debt-amount-slider">
                        <input type="radio" name="debt-amount" id="1" value="1" required>
                        <label for="1" data-debt-amount="< $25"></label>
                        <input type="radio" name="debt-amount" id="2" value="2" required>
                        <label for="2" data-debt-amount="$25-50"></label>
                        <input type="radio" name="debt-amount" id="3" value="3" required>
                        <label for="3" data-debt-amount="$50-100"></label>
                        <input type="radio" name="debt-amount" id="4" value="4" required>
                        <label for="4" data-debt-amount="$100-300"></label>
                        <input type="radio" name="debt-amount" id="5" value="5" required>
                        <label for="5" data-debt-amount="$300+ >"></label>
                        <div id="debt-amount-pos"></div>
                    </div>
                </form>
                <button type="submit">Cerca Prodotti</button>
            </div>

            <!-- fine price range bar -->

            <!-- brand list -->
            <div>
                <h4>BRAND</h4>
            </div>
            <ul class="list-group">
                <li v-for="brand in brands" :key="brand.title" class="list-group-item">
                    {{ brand.title }}
                    <span>
                        <input class="form-check-input" type="checkbox" id="checkboxNoLabel" value="" aria-label="...">
                    </span>
                </li>
            </ul>
            <!-- fine brand list -->

            <!-- color list -->
            <section>
                <h4>COLOR</h4>
                <div class="container d-flex gap-4 mt-2">
                    <div class="round">
                        <input type="checkbox" id="checkbox" />
                        <label for="checkbox" class="bg-primary"></label>
                    </div>
                    <div class="round">
                        <input type="checkbox" id="checkbox" />
                        <label for="checkbox" class="bg-danger"></label>
                    </div>
                    <div class="round">
                        <input type="checkbox" id="checkbox" />
                        <label for="checkbox" class="bg-success"></label>
                    </div>
                    <div class="round">
                        <input type="checkbox" id="checkbox" />
                        <label for="checkbox" class="bg-success"></label>
                    </div>
                    <div class="round">
                        <input type="checkbox" id="checkbox" />
                        <label for="checkbox" class="bg-success"></label>
                    </div>
                    <div class="round">
                        <input type="checkbox" id="checkbox" />
                        <label for="checkbox" class="bg-success"></label>
                    </div>
                    <div class="round">
                        <input type="checkbox" id="3" />
                        <label for="checkbox" class="bg-success"></label>
                    </div>
                </div>
            </section>

            <!-- fine color list -->
            <!-- inizio size bar -->
            <section class="mt-5">
                <h4>SIZE</h4>
                <div class="container d-flex gap-4 ">
                    <div class="round">
                        <input type="checkbox" id="checkbox" />
                        <label for="checkbox" class="bg-primary"></label>
                    </div>
                    <div class="round">
                        <input type="checkbox" id="checkbox" />
                        <label for="checkbox" class="bg-primary"></label>
                    </div>
                    <div class="round">
                        <input type="checkbox" id="checkbox" />
                        <label for="checkbox" class="bg-primary"></label>
                    </div>
                </div>
            </section>
            <!-- fine size bar -->
        </div>
        <!-- fine sidebar -->
    </div>
</template>

<script>
import { store } from '../store';
export default {
    data() {
        return {
            store,
            categories: [
                {
                    title: "Lifestyle",
                    state: "true",
                    badge:"4"
                },
                {
                    title: "Running",
                    state: "true",
                    badge:"9"
                },
                {
                    title: "Allenamento & Palestra",
                    state: "true",
                    badge:"5"
                },
                {
                    title: "Calcio",
                    state: "true",
                    badge:"11"
                },
                {
                    title: "Basketball",
                    state: "true",
                    badge:"3"
                },

            ],
            brands: [
                {
                    title: "Lifestyle",
                    state: "true",
                },
                {
                    title: "Running",
                    state: "true",
                },
                {
                    title: "Training & Gym",
                    state: "true",
                },
                {
                    title: "Basketball",
                    state: "false",
                },
            ],
        }
    }
}
</script>

<style lang="scss">
a {
    text-decoration: none;
    padding-right: 0.5rem;
}

.sidebar {
    display: flex;
    flex-direction: column;
    flex-shrink: 0;
    width: 400px;

}

.my-filter-bar {
    display: flex;
    width: 400px;
}

.my-border {
    border-right: 1px solid black;
    border-left: 1px solid black;
    border-bottom: 1px solid black;
}

.card-fix {
    padding-left: 0 !important;
    padding-right: 0 !important;
}
</style>