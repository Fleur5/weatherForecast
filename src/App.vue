<template>
  <header>
    <h1> Weather Forecast </h1>
  </header>
  <nav>
    <input 
        type="text" 
        placeholder="City name or zip code" 
        v-model="city_name"
        @keypress="fetchWeather"/>
  </nav>
  <main>
    <article>
    <h2> Krefeld </h2>
    <section>
      <h3> Current Weather </h3>
      <h4> Temperature </h4>
      <p> Current: </p>
      <p> Feels like: </p>
      <p> Pressure: </p>
      <p> Humidity: </p>
      <p> Cloudiness: </p>
      <p> UV index: </p>
      <h4> Wind </h4>
      <p> Wind speed: </p>
      <p> Wind gust: </p>
      <p> Wind degree: </p>
      <h4> Weather conditions </h4>
      <p> Current weather: </p>
      <p> WEATHER ICON </p>
      <p> Current rain: </p>
      <p> Current snow: </p>
    </section>
    <section>
      <h3> Forecast </h3>
      <h4> Date </h4>
      <p> Min temp: </p>
      <p> Max temp: </p>
      <p> WEATHER ICON </p>
    </section>
    <section>
      <h3> Alerts </h3>
      <p> Description </p>
      <p> Tags </p>
      <p> Start: </p>
      <p> End: </p>
      <p> Source: </p>
    </section>
    </article>
  </main>
  <footer>
  </footer>
</template>

<script>

export default {
  name: 'App',
  components: {
  
  },
  data(){
        return{
            city_name:''
        }
    },
    methods: {
      onInput(input){
        if(input.key == 'Enter') {
          // TODO Fetch weather for city_name
        }
      }
    },
    created(){
        // TODO Maybe fetch weather for placeholder (Berlin?)
      }
}
</script>

<style>

</style>
