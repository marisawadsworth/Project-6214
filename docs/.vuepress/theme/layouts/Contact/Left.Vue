<template>
    <div>
        <div class="contact-info">
        <div class="grid-container">
            <h1>Contact Form</h1> 
            <br>
                <form name="myForm" action="/action_page.html" method="GET">
                    First name:<br>
                    <!-- <input type="text" name="fname" required> -->
                    <input type="name" class="form-control" id="name" aria-describedby="fullname" placeholder="First name" required>
                    <small id="firstName" class="form-text text-muted"></small>
                    <br>
                    Last name:<br>
                    <!-- <input type="text" name="lname" required> -->
                    <input type="name" class="form-control" id="Fname" aria-describedby="fullname" placeholder="Last name" required>
                    <small id="lastName" class="form-text text-muted"></small>
                    <br>
                    Subject:<br>
                    <!-- <input type="text" name="comment" required> -->
                    <input type="subject" class="form-control" id="subject" placeholder="Your message" required>
                    <small id="text" class="form-text text-muted"></small>
                    <br>
                    Email:<br>
                    <!-- <input type="text" name"email" required> -->
                    <input type="email" class="form-control" id="exampleInputEmail1" placeholder="Enter email" required>
                    <small id="emailHelp" class="form-text text-muted"><p>I'll never share your email with anyone else.</p></small>
                    <br>
                    <input type="submit" value="Submit">
                </form>
            </div>
        </div>
        <Content />
    </div>
</template>

<script>
    export default {
        name: 'Left'
    }
</script>

<style lang="css" scoped>

</style>