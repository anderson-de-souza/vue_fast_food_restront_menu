
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
        width: 100vw;
        min-height: 128px;
        background-color: black;
        color: gold;
        display: flex;
        align-items: center;
        justify-content: space-around;
        flex-wrap: wrap;
    }

    ul {
        min-width: 350px;
        list-style: none;
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    a:hover {
        text-decoration: underline;
    }

    a {
        text-decoration: none;
        color: gold;
    }

</style>
