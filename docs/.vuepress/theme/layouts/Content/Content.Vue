<template>
    <main>
    <h1>Links</h1>
    <br>

    <a href="https://www.accuweather.com/en/nz/tauranga/246959/weather-forecast/246959" class="aw-widget-legal">
      <!--
      By accessing and/or using this code snippet, you agree to AccuWeather’s terms and conditions (in English) which can be found at https://www.accuweather.com/en/free-weather-widgets/terms and AccuWeather’s Privacy Statement (in English) which can be found at https://www.accuweather.com/en/privacy.
      -->
      </a><div id="awcc1536196043169" class="aw-widget-current"  data-locationkey="246959" data-unit="c" data-language="en-us" data-useip="true" data-uid="awcc1536196043169"></div><script type="text/javascript" src="https://oap.accuweather.com/launch.js"></script>

      <p>
        <a href="https://toiohomai.ac.nz/">
        <img :src="Toiohomailogo" alt="toiohomai" class="toiohomai">
        <Content />
        </a>
      </p>
        </section>
    </main>
</template>

<script>
    import Logo from '../../../public/images/toiohomai.jpg'
    export default {
        name: 'Content',
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
    width: 50%;
    height: 300px;
}
</style>