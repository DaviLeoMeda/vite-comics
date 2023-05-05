<script>
export default {
    name: "DcFooter",

}
</script>

<template>
    <div id="backFooter">
        <div class="container">
            <div>
                <h4>dc comics</h4>
                <ul>
                    <li><a href="#">Characters</a></li>
                    <li><a href="#">Comics</a></li>
                    <li><a href="#">Movies</a></li>
                    <li><a href="#">TV</a></li>
                    <li><a href="#">Games</a></li>
                    <li><a href="#">Videos</a></li>
                    <li><a href="#">News</a></li>
                </ul>
                <h4>shop</h4>
                <ul>
                    <li>
                        <a href="#">Shop DC</a>
                    </li>
                    <li>
                        <a href="#">Shop DC Collectibles</a>
                    </li>
                </ul>
            </div>
            <div>
                <h4>dc</h4>
                <ul>
                    <li><a href="#">Terms of Use</a></li>
                    <li><a href="#">Privacy Policy(New)</a></li>
                    <li><a href="#">Ad Choices</a></li>
                    <li><a href="#">Advertising</a></li>
                    <li><a href="#">Jobs</a></li>
                    <li><a href="#">Subscruptions</a></li>
                    <li><a href="#">Talent Workshops</a></li>
                    <li><a href="#">CPSC Certifications</a></li>
                    <li><a href="#">Ratings</a></li>
                    <li><a href="#">Shop Help</a></li>
                    <li><a href="#">Contact Us</a></li>
                </ul>
            </div>
            <div>
                <h4>sites</h4>
                <ul>
                    <li><a href="#">DC</a></li>
                    <li><a href="#">MAD Magazine</a></li>
                    <li><a href="#">DC Kids</a></li>
                    <li><a href="#">DC Universe</a></li>
                    <li><a href="#">DC Power Visa</a></li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style scooped lang="scss">
#backFooter {
    background-image: url(../../public/img/footer-bg.jpg);
}

.container {
    display: flex;

    div {
        padding: 30px;

        h4 {
            text-transform: uppercase;
            color: #fff;
            padding: 20px 0;
        }

        ul {
            li {
                list-style-type: none;
                padding: 3px 0;

                a {
                    text-decoration: none;
                    color: gray;
                }
            }
        }
    }
}
</style>