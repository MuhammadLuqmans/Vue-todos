<script setup lang="ts">
import 'bootstrap/dist/js/bootstrap.js'
import { RouterLink, RouterView } from 'vue-router'

</script>
<template>
    <nav class="col-12 navbar navbar-expand-lg navbar-dark bg-dark px-4">
        <a class="navbar-brand" href="#">Navbar</a>
        <button
            class="navbar-toggler"
            type="button"
            data-toggle="collapse"
            data-target="#navbarSupportedContent"
            aria-controls="navbarSupportedContent"
            aria-expanded="false"
            aria-label="Toggle navigation"
        >
            <span class="navbar-toggler-icon"></span>
        </button>

        <div class="collapse navbar-collapse d-flex align-item-center justify-content-between" id="navbarSupportedContent">
            <ul class="navbar-nav mr-auto">
                <li class="nav-item active">
                    <a class="nav-link" href="#">
                        <RouterLink to="/">Home</RouterLink>
                    </a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" href="#">
                        <RouterLink to="/about">About</RouterLink>
                    </a>
                </li>
                <li class="nav-item dropdown">
                           <RouterLink to="/contact">Contact us</RouterLink>
                </li>
                <li class="nav-item">
                    <a
                        class="nav-link disabled"
                        href="#"
                        tabindex="-1"
                        aria-disabled="true"
                    >Disabled</a>
                </li>
            </ul>
            <form class="form-inline my-2 my-lg-0 d-flex justify-content-between border-orange">
                <input
                    class="form-control mr-sm-2"
                    type="search"
                    placeholder="Search"
                    aria-label="Search"
                />
                <button class="btn btn-outline-success m-2 my-sm-0" type="submit">Search</button>
            </form>
        </div>

    </nav>
</template>