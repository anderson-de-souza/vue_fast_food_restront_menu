
<template>

    <header>
        <h1>{{ title }}</h1>
        <nav>
            <ul>
                <li>
                    <a href="#">Foods</a>
                </li>
                <li>
                    <a href="#">Hambuguers</a>
                </li>
                <li>
                    <a href="#">Hot Dogs</a>
                </li>
                <li>
                    <a href="#">Drinks</a>
                </li>
            </ul>
        </nav>
    </header>

</template>

<script>
    export default {
        name: 'HeaderComponent',
        props: {
            title: String
        }
    }
</script>

<style scoped>

    header {
        max-width: 1200px;
        height: 180px;
        margin: 0 auto;
        padding: 0 24px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        flex-wrap: wrap;
    }

    h1 {
        color: brown;
        font-size: 2.25rem;
    }

    ul {
        min-width: 380px;
        list-style: none;
        display: flex;
        justify-content: space-between;
    }

    a {
        color: brown;
        font-size: 1.25rem;
        text-decoration: none;
        font-weight: bold;
    }

    a:hover {
        color: black;
        text-decoration: underline;
    }

</style>
