<template>
    <div>
        <footer>
            <div class="container">
                <div class="footer-item">
                    <h4>VISIT A PGX STORE</h4>
                    <hr>
                    <ul>
                        <li>
                            <a href="#">BOSTON</a>
                        </li>
                        <li>
                            <a href="#">CHARLOTTE</a>
                        </li>
                        <li>
                            <a href="#">CHICAGO NORTH</a>
                        </li>
                        <li>
                            <a href="#">CHICAGO WEST</a>
                        </li>
                        <li>
                            <a href="#">CINCINNATI</a>
                        </li>
                        <li>
                            <a href="#">DALLAS</a>
                        </li>
                        <li>
                            <a href="#">DENVER</a>
                        </li>
                        <li>
                            <a href="#">DETROIT</a>
                        </li>
                        <li>
                            <a href="#">CHICAGO WEST</a>
                        </li>
                    </ul>
                </div>
                <div class="footer-item">
                    <h4>ABOUT</h4>
                    <hr>
                    <ul>
                        <li>
                            <a href="#">ABOUT PGX</a>
                        </li>
                        <li>
                            <a href="#">BLOG</a>
                        </li>
                        <li>
                            <a href="#">OUR FOUNDER</a>
                        </li>
                        <li>
                            <a href="#">CAREERS</a>
                        </li>
                    </ul>
                </div>
                <div class="footer-item">
                    <h4>LEGAL AND POLICIES</h4>
                    <hr>
                    <ul>
                        <li>
                            <a href="#">SHIPPING INFORMATION</a>
                        </li>
                        <li>
                            <a href="#">PRIVACY POLICY</a>
                        </li>
                        <li>
                            <a href="#">RETURN POLICY</a>
                        </li>
                    </ul>
                </div>
                <div class="footer-item">
                    <h4>FOLLOW US</h4>
                    <hr>
                    <ul>
                        <li>
                            <a href="#" class="social-media"><font-awesome-icon icon="fa-brands fa-facebook-square"></font-awesome-icon></a>
                            <a href="#" class="social-media"><font-awesome-icon icon="fa-brands fa-twitter-square"></font-awesome-icon></a>
                            <a href="#" class="social-media"><font-awesome-icon icon="fa-brands fa-instagram-square"></font-awesome-icon></a>
                        </li>
                    </ul>
                </div>
            </div>
        </footer>
    </div>
</template>

<script>
export default {
    setup() {

    }
}
</script>

<style scoped>
footer {
    background-color: #000;
    padding-bottom: 4rem;
}

.footer-item {
    text-align: left;
    padding: 1rem 1.5rem 0;
}

.container {
    max-width: 1000px;
    color: #fff;
    margin: auto;
}

li {
    font-size: 14px;
    margin-bottom: 0.5rem;
}

.social-media {
    margin-right: 1.5rem;
    font-size: 20px;
}

@media only screen and (min-width: 800px) {
    .container {
        display: grid;
        grid-template-columns: repeat(4, 1fr);
    }
}
</style>