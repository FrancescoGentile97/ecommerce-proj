<template>
    <section>
        <div class="w-100 my-secondary">
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

    <div class="container flex-grow-1 my-p-unset">
        <div class="row">
            <div class="col-4">
                <div class="d-flex flex-column mb-3">
                    <!-- lista delle categorie -->
                    <ul class="list-group">
                        <div class="list-group-item d-flex justify-content-between align-items-start">
                            <div class="fw-bold">
                                <h5>CATEGORIES</h5>
                            </div>
                        </div>
                        <li v-for="category in categories" :key="category.title"
                            class="list-group-item d-flex justify-content-between align-items-start">
                            {{ category.title }}
                            <span class="badge bg-primary rounded-pill">
                                {{ category.badge }}
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
                    <li v-for="brand in brands" :key="brand.title"
                        class="list-group-item d-flex justify-content-between align-items-start">
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
                    <!-- <div class="container d-flex gap-4 mt-2">
                        <div class="round">
                            <input type="checkbox" id="10" />
                            <label for="10" class="bg-primary"></label>
                        </div>
                        <div class="round">
                            <input type="checkbox" id="11" />
                            <label for="11" class="bg-danger"></label>
                        </div>
                        <div class="round">
                            <input type="checkbox" id="12" />
                            <label for="12" class="bg-success"></label>
                        </div>
                        <div class="round">
                            <input type="checkbox" id="13" />
                            <label for="13" class="my-primary"></label>
                        </div>
                        <div class="round">
                            <input type="checkbox" id="14" />
                            <label for="14" class="bg-success"></label>
                        </div>
                        <div class="round">
                            <input type="checkbox" id="15" />
                            <label for="15" class="bg-success"></label>
                        </div>
                        <div class="round">
                            <input type="checkbox" id="16" />
                            <label for="16" class="bg-success"></label>
                        </div>
                    </div> -->
                    <div class="row">
                        <div v-for:="color in colorsList" :key="i" class="col-3">
                            <div class="round">
                                <input type="checkbox" id="{{ color.id }}">
                                <label for="{{ color.for }}" class="bg-primary"></label>
                            </div>
                        </div>
                    </div>
                </section>

                <!-- fine color list -->
                <!-- inizio size bar -->
                <section class="mt-5">
                    <h4>SIZE</h4>
                    <div class="row">
                        <div v-for:="size in sizesList" :key="i" class="col-3">
                            <div class="round">
                                <input type="checkbox" id="{{ size.id }}">
                                <label for="{{ size.for }}" class="bg-primary">{{ size.size }}</label>
                            </div>
                        </div>
                    </div>
                </section>
                <!-- fine size bar -->
            </div>
            <!-- fine side bar -->

            <!-- inizio main content -->
            <div class="col-8">
                <div class="row">
                    <div v-for:="product, i  in productList" :key="i" class="col-3 mt-2">
                        <div class="card">
                            <div class="position-relative">
                                <img v-bind:src="product.image" class="img-fluid">
                            </div>
                            <h5>{{ product.name }}</h5>
                            <p>{{ product.price }}</p>
                            <div class="position-absolute top-0 text-white ">
                                <div class="mt-2 ms-2  bg-black ">
                                    {{ product.sold }}
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <nav aria-label="Page navigation example" class="d-flex justify-content-center mt-2">
                    <ul class="pagination">
                        <li class="page-item">
                            <a class="page-link" href="#" aria-label="Previous">
                                <span aria-hidden="true">&laquo;</span>
                            </a>
                        </li>
                        <li class="page-item"><a class="page-link" href="#">1</a></li>
                        <li class="page-item"><a class="page-link" href="#">2</a></li>
                        <li class="page-item"><a class="page-link" href="#">3</a></li>
                        <li class="page-item"><a class="page-link" href="#">4</a></li>
                        <li class="page-item"><a class="page-link" href="#">5</a></li>
                        <li class="page-item">
                            <a class="page-link" href="#" aria-label="Next">
                                <span aria-hidden="true">&raquo;</span>
                            </a>
                        </li>
                    </ul>
                </nav>
            </div>

            <!-- fine main content -->
        </div>
    </div>
    <!-- fine sidebar -->
</template>

<script>
import { store } from '../store';
export default {
    data() {
        return {
            store,
            sizesList: [
                {
                    type: "checkbox",
                    id: "17",
                    for: "17",
                    size: "37",
                },
                {
                    type: "checkbox",
                    id: "18",
                    for: "18",
                    size: "38",
                },
                {
                    type: "checkbox",
                    id: "19",
                    for: "19",
                    size: "39",
                },
                {
                    type: "checkbox",
                    id: "20",
                    for: "20",
                    size: "40",
                },
                {
                    type: "checkbox",
                    id: "21",
                    for: "21",
                    size: "41",
                },
                {
                    type: "checkbox",
                    id: "22",
                    for: "22",
                    size: "42",
                },
                {
                    type: "checkbox",
                    id: "23",
                    for: "23",
                    size: "43",
                },
                {
                    type: "checkbox",
                    id: "24",
                    for: "24",
                    size: "44",
                },
            ],
            colorsList: [
                {
                    type: "checkbox",
                    id: "11",
                    for: "11",
                    class: "color-list-green",
                },
                {
                    type: "checkbox",
                    id: "12",
                    for: "12",
                    class: "color-list-black",
                },
                {
                    type: "checkbox",
                    id: "13",
                    for: "13",
                    class: "color-list-blue",
                },
                {
                    type: "checkbox",
                    id: "14",
                    for: "14",
                    class: "color-list-purple",
                },
                {
                    type: "checkbox",
                    id: "15",
                    for: "15",
                    class: "color-list-orange",
                },
                {
                    type: "checkbox",
                    id: "16",
                    for: "16",
                    class: "",
                },
                {
                    type: "checkbox",
                    id: "16",
                    for: "16",
                    class: "",
                },
                {
                    type: "checkbox",
                    id: "16",
                    for: "16",
                    class: "",
                },
            ],
            productList: [
                {
                    name: "Jordan Max Aura 4",
                    image: "/src/assets/jordan-1.png",
                    price: "129,99$",
                    sold: "-20%",
                },
                {
                    name: "Air Jordan 5 Retro",
                    image: "/src/assets/scarpa-air-jordan-5-retro.jpeg",
                    price: "209,99$",
                    sold: "-10%",
                },
                {
                    name: "Jordan 1 Mid",
                    image: "/src/assets/jordan-1-mid.webp",
                    price: "89,99$",
                    sold: "-30%",
                },
                {
                    name: "Air Jordan 1 Zoom CMFT 2",
                    image: "/src/assets/Air Jordan 1 Zoom CMFT 2.webp",
                    price: "159,99$",
                    sold: "",
                },
                {
                    name: "Air Jordan 1 Elevate High",
                    image: "/src/assets/Air Jordan 1 Elevate High.webp",
                    price: "149,99$",
                    sold: "-10%",
                },
                {
                    name: "Air Jordan 1 White Cement",
                    image: "src/assets/Air Jordan 1 White Cement.webp",
                    price: "179,99$",
                    sold: "",
                },
                {
                    name: "Air Jordan Legacy 312 Low",
                    image: "/src/assets/Air Jordan Legacy 312 Low.webp",
                    price: "89,99$",
                    sold: "-40%",
                },
                {
                    name: "Jordan Jumpman Pro",
                    image: "/src/assets/Jordan Jumpman Pro.webp",
                    price: "145,99$",
                    sold: "-20%",
                },
            ],
            categories: [
                {
                    title: "Lifestyle",
                    state: "true",
                    badge: "4"
                },
                {
                    title: "Running",
                    state: "true",
                    badge: "9"
                },
                {
                    title: "Allenamento & Palestra",
                    state: "true",
                    badge: "5"
                },
                {
                    title: "Calcio",
                    state: "true",
                    badge: "11"
                },
                {
                    title: "Basketball",
                    state: "true",
                    badge: "3"
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

.my-filter-bar {
    display: flex;
    flex-shrink: 0;
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