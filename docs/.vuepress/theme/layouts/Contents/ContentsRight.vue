<template>
    <div>
        <img :src="Toiohomailogo" alt="Toiohomailogo" class="toiohomai"/>
    </div>
</template>

<script>
    import Logo from '../../../public/images/toiohomai.jpg'
    export default {
        name: 'toiohomai',
        data() {
            return {
                Toiohomailogo: Logo
            }
        }
    }
</script>

<style lang="css" scoped>

.toiohomai {
    display: block;
    width: 500px;
    height: 250px;
    float: right;
    padding: 20px;
}
</style>