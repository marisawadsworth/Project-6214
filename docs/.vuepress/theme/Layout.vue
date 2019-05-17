<template>
    <div>
        <div class = "header-logo">
            <img :src="logo" alt="logo" />
        </div>

        <nav>Navigation</nav>

        <main>
            <section class="left">
                <Left />
            </section>
            <section class="right">
                <Right />
            </section>
        </main>

        <footer>
            <p>Marisa Wadsworth</p>
        </footer>

    </div>
</template>

<script>
    import Left from '../theme/layouts/Left'
    import Right from '../theme/layouts/Right'
    import Logo from '../public/images/logo.png'
    export default {
        components : {
            Left,
            Right
        },
        data() {
            return {
                logo: Logo
            }
        }
    }
</script>

<style lang="css">
html, body {
    margin : 0;
    padding: 0;
    height: 100%;
    font-family: Arial, Helvetica, sans-serif;
}

.header-logo{
    display: grid;
    grid-template-columns: 1fr;
    justify-items: center;
    align-content: center;
    height: 200px;
    background-color: pink;
}

nav {
    display: grid;
    grid-template-columns: 1fr;
    justify-items: center;
    align-content: center;
    height: 50px;

    background-color: rgb(181, 77, 165);
    color: white;
}

main {
    display: grid;
    grid-template-columns: 1fr 1fr;
    height: 100%;
}

.left {
    display: grid;
    grid-template-columns: 1fr;
    padding: 20px;
    box-sizing: border-box;
    height: 100%;

    background-color: #efefef;
    color: #222;
}

.right {
    display: grid;
    grid-template-columns: 1fr;
    padding: 20px;
    box-sizing: border-box;
    height: 100%;

    background-color: #898989;
    color: #222;
}

footer {
    display: grid;
    grid-template-columns: 1fr;
    justify-items: center;
    align-content: center;
    height: 50px;

    position: absolute;
    bottom: 0;
    width: 100%;

    background-color: #777;
    color: white;
}

@media screen and (max-width: 640px) {
    main {
        grid-template-columns: 1fr;
    }       
}

</style>