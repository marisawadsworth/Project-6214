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
    import Left from './ContentsLeft'
    import Right from './ContentsRight'

    export default {
        name: 'Toiohomai',
        props: {
            name: 'Toiohomai'
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
</style>
