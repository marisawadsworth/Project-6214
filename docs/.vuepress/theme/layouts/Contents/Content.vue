<template>
    <main>
        <!-- <img :src="Toiohomailogo" alt="logo" /> -->
        <Content />
    </main>
</template>

<script>
console.log("TESTING!")
    import Logo from '../../../public/images/toiohomai.jpg'
    export default {
        name: 'content',
        data() {
            return {
                Toiohomailogo: Logo
            }
        }
    }
</script>

<style lang="css" scoped>

main {
    display: grid;
    grid-template-columns: 1fr 1fr;
    height: 100%;
}

.toiohomai {
    display: block;
    width: 50%;
    height: 300px;
}

</style>