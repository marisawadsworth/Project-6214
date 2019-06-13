<template>
    <div>
        <img :src="profilepic" alt="Me" class="profilepic">
    </div>
</template>

<script>
    import Logo from '../../../public/images/profilepic.jpg'
    export default {
        name: 'Right',
        data() {
            return {
                profilepic: Logo
            }
        }
    }
</script>

<style lang="css" scoped>

.profilepic{
    width: 300px;
    height: 300px;
    /* float: right; */
    margin: 20px;
    /* border: 2px solid black; */
}
</style>