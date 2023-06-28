<template>
    <div>
        <header>
            <div class="logo">
                <img src="https://i.postimg.cc/Mpqd0qt3/Screenshot-2023-06-09-120627.png" alt="Logo">
            </div>
            <nav>
                <ul class="nav-links">
                    <router-link class="active" to="/">Home</router-link>
                    <router-link to="/products">Products</router-link>
                    <router-link to="/about">About</router-link>
                    <router-link to="/admin">Admin</router-link>

                </ul>
            </nav>
        </header>
    </div>
</template>
<script>
export default {

}
</script>
<style></style>