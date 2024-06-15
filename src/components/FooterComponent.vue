
<template>
    <footer>
        
        <span>anderson-de-souza&copy; 2024</span>

        <ul>
            <li>
                <a>
                    <i class="fab fa-facebook"></i>
                </a>
            </li>
            <li>
                <a>
                    <i class="fab fa-instagram"></i>
                </a>
            </li>
            <li>
                <a>
                    <i class="fab fa-twitter"></i>
                </a>
            </li>
            <li>
                <a>
                    <i class="fab fa-whatsapp"></i>
                </a>
            </li>
            <li>
                <a>
                    <i class="fab fa-telegram"></i>
                </a>
            </li>
        </ul>

    </footer>
</template>

<script>
    
    export default {
        name: 'FooterComponent'
    }

</script>

<style scoped>

    @import url('@fortawesome/fontawesome-free/css/all.css');

    footer {
        max-width: 1200px;
        height: 180px;
        margin: 0 auto;
        padding: 0 24px;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    span {
        color: brown;
        font-weight: 900;
    }

    ul {
        min-width: 150px;
        list-style: none;
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    i {
        color: brown;
        scale: 1.4;
    }

</style>