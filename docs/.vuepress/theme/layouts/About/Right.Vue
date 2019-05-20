<template>
    <div>
        <img :src="profilepic" alt="Me" class="profilepic">
    </div>
</template>

<script>
    import Logo from '../public/images/profilepic.png'
    export default {
        name: "Right"
    }
</script>

<style lang="css" scoped>

.profilepic{
    width: 250px;
    height: 250px;
    /* float: right; */
    margin: 20px;
    border: 2px solid black;
}
</style>