<template>

<div id="app" v-cloak>
    <div class="widget"> TU BEDZIE JAKIES LOGO CZY NAZWA</div>

  <div class="widget" v-if="errorStr">
    Sorry, but the following error
    occurred: {{errorStr}}
  </div>

  <div class="widget" v-if="gettingLocation">
    <i>Getting your location...</i>
  </div>

  <div class="widget" v-if="location">
    Your location data is [[ location.coords.latitude ]], [[ location.coords.longitude]]
  </div>

    <div class="widget" v-if="place">
        Najbliższa placówka to [[place]], znajduje się w odległości [[distance]]


    </div>
    <div class="widget">
        Czy to ptak? Czy to samolot? Nie, tu będzie wykresik


    </div>

</div>

</template>