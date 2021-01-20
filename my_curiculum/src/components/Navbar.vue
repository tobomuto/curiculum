<template>
<b-container>
    <b-navbar type="white" class="fixed-top">
        <b-navbar-brand class="logo" href="/">TOMBVR</b-navbar-brand>

        <b-navbar-nav class="ml-auto">
            <b-nav-item href="#second">About</b-nav-item>
            <b-nav-item href="#chronologie">Chronologie</b-nav-item>
            <b-nav-item href="#fourth">Contact</b-nav-item>
        </b-navbar-nav>

    </b-navbar> 
</b-container>
</template>

<script>
export default {
    name: 'Navbar'

}
</script>

<style>

.logo {
    color: white;
    font-family: 'Marcellus', serif;
}

.ml-auto {
    font-family: 'Lato', sans-serif;
}
.logo:hover {
    color: rgb(255, 255, 255);
}

.nav-link {
    color: white;
    font-family: 'Lato', sans-serif;
    transition: 0.5s;
}

.nav-link:hover {
    color: rgb(33, 36, 37);
    background-color: white;
    border-radius: 30px;
}
</style>