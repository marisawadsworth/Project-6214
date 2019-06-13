<template>
    <div>
        <div class = "header-logo">
            <img :src="logo" alt="logo" />
        </div>

        <nav>Navigation</nav>
        <nav class="navbar navbar-expand-lg navbar-light bg-light">
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
    
      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav mr-auto">
          <li class="nav-item active">
            <a class="nav-link" href="/index.html">Home <span class="sr-only">(current)</span></a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="/pages/about/">About Me</a>
          </li>
          <li class="nav-item dropdown">
            <a class="nav-link dropdown-toggle" href="#" id="navbarDropdowncourse" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
              Course
            </a>
            <div class="dropdown-menu" aria-labelledby="navbarDropdown">
                  <a class="dropdown-item" href="/pages/course/5209.html">5209</a>
                  <a class="dropdown-item" href="/pages/course/5210.html">5210</a>
                  <a class="dropdown-item" href="/pages/course/5211.html">5211</a>
                  <a class="dropdown-item" href="/pages/course/6209.html">6209</a>
                  <a class="dropdown-item" href="/pages/course/6210.html">6210</a>
            </div>
          </li>
          <li class="nav-item dropdown">
          <a class="nav-link dropdown-toggle" href="#" id="navbarDropdowncontent" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
              Content
          </a>
          <div class="dropdown-menu" aria-labelledby="navbarDropdown">
                  <a class="dropdown-item" href="/pages/content/links.html">Links</a>
                  <a class="dropdown-item" href="/pages/content/policy.html">Policy</a>
              <div class="dropdown-divider"></div>
                  <a class="dropdown-item" href="content/toiohomai.html">Toi Ohomai</a>
              </div>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="/pages/contact/contactform.html">Contact</a>
          </li>
        </ul>
      </div>
    </nav>

    <!-- {{ WhatPage }} -->

        <component :is="WhatPage" />

        <footer>
            <p>Marisa Wadsworth</p>
        </footer>

    </div>
</template>

<script>
    import Home from './layouts/Home/Main'
    import About from './layouts/About/Main'
    import Course from './layouts/Course/Main'
    import Contents from './layouts/Contents/'
    import Contact from './layouts/Contact/Main'
    import Logo from '../public/images/logo.png'

    //import 'bootstrap'
    import 'bootstrap/dist/css/bootstrap.min.css'

    export default {
        name: "Layout",
        components: {
            Home,
            About,
            Course,
            Contents,
            Cont
        },
        data() {
            return {
                logo: Logo
            }
        },
        computed: {

            WhatPage(){
                console.log(this.$options.parent.$page.frontmatter.layout)
                return this.$options.parent.$page.frontmatter.layout
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


footer {
    display: grid;
    grid-template-columns: 1fr;
    justify-items: center;
    align-content: center;
    height: 50px;

    position: absolute;
    /* bottom: 0; */
    width: 100%;

    background-color: #777;
    color: white;
}

</style>