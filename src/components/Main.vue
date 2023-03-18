<template>
    <main>
        <section>
            <div class="">
                <!-- link del catalogo -->
                <div class="my-primary text-center">
                    <h3>Scarpe Uomo</h3>
                    <a href="">Home</a>
                    <a href="">Catalogo</a>
                    <a href="">Uomo</a>
                </div>
            </div>
        </section>

        <!-- fine link catalogo -->




        <!-- new section -->
        <div class="row">
            <div class="col-7 card-fix">
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
            <div class="col-5 card-fix">
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
        </div>
        <!-- fine new section -->

        <!-- toolbar -->

        <div class="row">
            <div class="col">1</div>
            <div class="col">2</div>
            <div class="col">3</div>
            <div class="col">4</div>
        </div>
        <!-- fine tooblar -->

        <!-- sidebar categories... -->
        <div class="sidebar">
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
                <H4>SIZE</H4>
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

    </main>
</template>

<script>
import { store } from '../store';
export default {
    data() {
        return {
            store,
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