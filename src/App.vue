<template>
  <div id="app">
    <main>
      <div class="search-box">
        <input type="text" name="" id="" class="search-bar" placeholder="Search.." />

      </div>

      <div class="weather-wrap">
        <div class="location-box">
          <div class="location">São Paulo, BR</div>
          <div class="date">Segunda 20 de março de 2023</div>
        </div>

        <div class="weather-box">
          <div class="temp">9 C</div>
          <div class="weather">Rain</div>
        </div>
        
      </div>
    </main>

  </div>
</template>

<script>
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'app',
  data() {
    return {
      api_key: '9e13a0075fb1aa385412e90c625b562e'
    }
  }
})

</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'montserrat', sans-serif;

}

#app {
  background-image: url('./assets/cold-bg.jpg');
  background-size: cover;
  background-position: center;
  transition: 0.4;
  background-repeat: no-repeat;
  border-radius: 25px;
  width: 400px;


}

main {
  min-height: 70vh;
  padding: 25px;
  background-image: linear-gradient(rgba(0, 0, 0, 0.25), rgba(0, 0, 0, 0.75));
  border-radius: 25px;

}

.search-box {
  width: 100%;
  text-align: center;

}

input {
  border-radius: 0px 16px 0px 16px;
  width: 170px;
  text-align: center;
  height: 32px;
  appearance: none;
  border: none;
  outline: none;
  background: none;
  box-shadow: 0px 0px 0px rgba(0, 0, 0, 0.25);
  transition: 0.4s;
}

.search-box .search-bar {
  box-shadow: 0px 0px 16px;
  background-color: rgba(255, 255, 255, 0.75);
  border-radius: 16px, 0px, 16px, 0px;
}

.location-box .location {
  color: #FFF;
  font-size: 18px;
  font-weight: 500;
  text-align: center;
  text-shadow: 1px 3px rgba(0, 0, 0, 0.25);
  margin-top: 15px;
}

.location-box .date {
  color: #FFF;
  font-size: 10px;
  font-weight: 300;
  font-style: italic;
  text-align: center;
}

.weather-box {
  text-align: center;

}

.weather-box .temp {
  display: inline-block;
  padding: 10px 25px;
  color: #FFF;
  font-size: 48px;
  font-weight: 700;
  text-shadow: 3px 6px rgba(0, 0, 0, 0.25);
  background-color: rgba(255, 255, 255, 0.25);
  border-radius: 16px;
  margin: 30px 0px;
  box-shadow: 3px 6px rgba(0, 0, 0, 0.25);

}

.weather-box .weather {
  color: #FFF;
  font-size: 24px;
  font-weight: 350;
  font-style: italic;
  text-shadow: 3px 6px rgba(0, 0, 0, 0.25);
}
</style>
