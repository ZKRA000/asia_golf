<template>
    <div>
        <nav>
            <div class="container">
                <div class="img">
                    <img src="./../assets/pxg.svg" alt="">
                </div>
                <div class="toggle">
                    <font-awesome-icon icon="fa-solid fa-bars"></font-awesome-icon>
                </div>
                <ul class="navbar-items">
                    <li><a href="#">HOME</a></li>
                    <li><a href="#">ABOUT US</a></li>
                    <li><a href="#">HOW TO BUY</a></li>
                    <li><a href="#">STORE LOCATION</a></li>
                    <li><a href="#">BRANDS</a></li>
                    <li><a href="#">CONTACT US</a></li>
                </ul>
            </div>
        </nav>
    </div>
</template>

<script>
export default {
    name:'MyNavbar'
}
</script>

<style scoped>
nav {
    background-color: black;
    border-bottom: 2px solid #fff;
}

.container {
    display: flex;
    margin: 0 auto;
    justify-content: center;
    align-items: center;
    padding: 0 2rem;
    max-width: 1000px;
}

.img {
    padding: 1rem 0;
}

.toggle {
    display: none;
    color: #fff;
    font-size: 20px;
}

ul {
    display: flex;
}

ul li {
    padding: 20px;
}

li:hover {
    background-color: #171717;
}

img {
    width: auto;
    height: 30px;
}

a {
    color: #fff;
}

@media only screen and (max-width: 800px) {
    .navbar-items {
        display: none;
    }

    .container {
        justify-content: space-between;
    }

    .toggle {
        display: block;
    }
}
</style>