<template>
    <main>
        <section class="left">
            <Left />
        </section>
        <section class="right">
            <Right />
        </section>
    </main>
</template>

<script>
    import Left from './AboutLeft'
    import Right from './AboutRight'

    export default {
        name: 'About',
        props: {
            name: 'About'
        },
        components : {
            Left,
            Right
        }
    }
</script>

<style lang="css" scoped>
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

@media screen and (max-width: 640px) {
    main {
        grid-template-columns: 1fr;
    }       
}
</style>