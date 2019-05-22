**GOOGLE MAP**

1- Log on to https://console.cloud.google.com

2- Create a new project

3- Click on the nav menu

4- Select API & Services

5- Click on "Enable API & Services"

6- All google services you can use will be listed, select MAP JS API

7- Click on "Enable"

8- Click on "Credentials"

9- Click on "Create Credentials"

10- Select "Create API Key"

11- Copy the key and keep somewhere

12- Go to https://developers.google.com/maps/documentation/javascript/tutorial to view the docs for creating a map

13- JS map code { Add this to the main.js file imported to the index.html }

`//Initialize and add the map function initMap() { //Your location const loc = { lat: 6.524379, lng: 3.379206 }; //centered map on location const map = new google.maps.Map(document.querySelector(".map"), { zoom: 14, center: loc }); // The marker, positioned at location const market = new google.maps.Market({ position: loc, map: map }); }`

14- Above the body tag, add this

    <script src="js/main.js"></script>
    <script
      src="https://maps.googleapis.com/maps/api/js?key=AIzaSyAiXac5RreTzlg9zpWLrFbJXZ0Cb9uQdUc&callback=initMap"
      async
      defer
    ></script>
