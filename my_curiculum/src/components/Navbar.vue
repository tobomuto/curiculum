<template>
<b-container>
    <b-navbar type="white">
        <b-navbar-brand class="logo" href="/">TOMBVR</b-navbar-brand>

        <b-navbar-nav class="ml-auto">
            <b-nav-item href="#second">About</b-nav-item>
            <b-nav-item href="#third">Experiences</b-nav-item>
            <b-nav-item href="#fourth">Studies</b-nav-item>
            <b-nav-item href="#fifth">Contact</b-nav-item>
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

.logo:hover {
    color: rgb(255, 255, 255);
}

.nav-link {
    color: white;
    font-family: 'Marcellus', serif;
    transition: 0.4s;
}

.nav-link:hover {
color: teal;
}
</style>