<template>
    <div>
        <img :src="profilepic" alt="Me" class="contact-img">
    </div>
</template>

<script>
    import Logo from '../../../public/images/me.jpg'
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

.contact-img{
    width: 450px;
    float: right;
    margin: 20px;
    margin-top: 50px;
    margin-right: 50px;
}

</style>
