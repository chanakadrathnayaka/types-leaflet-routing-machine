# TypeScript definition for leaflet routing machine

Leaflet Routing Machine is an amazing plugin developed by [@perliedman](https://github.com/perliedman/leaflet-routing-machine) in order to draw routes on a leaflet map. TypeScript definition helps you to use this plugin in your typescript projects.

## How to use leaflet-routing-machine.js in an Angular project 

1. Install [_leaflet_](https://www.npmjs.com/package/leaflet)
    ```npm
        npm i leaflet
    ```
2. Install [_TypeScript definition of leaflet_](https://www.npmjs.com/package/@types/leaflet)
    ```npm
        npm i --save-dev @types/leaflet
    ```
3. Install [_leaflet routing machine_](https://www.npmjs.com/package/leaflet-routing-machine)
    ```npm
        npm i leaflet-routing-machine
    ```
4. Install [_TypeScript definition of leaflet routing machine_](https://www.npmjs.com/package/@types/leaflet-routing-machine)
    ```npm
        npm i --save-dev @types/leaflet-routing-machine
    ```
5. Import leaflet.css & leaflet-routing-machine.css into the project
    - Open angular-cli.json
    - Add leaflet & leaflet-routing-machine css file into style attribute.
    ```javascript
        "styles": [
            "../node_modules/leaflet/dist/leaflet.css",
            "../node_modules/leaflet-routing-machine/dist/leaflet-routing-machine.css"
        ]
    ```
6. Import leaflet into the component
    - Add below import statements top of your component
    ```javascript
        import * as L from 'leaflet';
        import 'leaflet-routing-machine';
    ```
    
## How to use leaflet routing machine in your typescript project

```javascript
import * as L from 'leaflet';
import 'leaflet-routing-machine';

const map: L.Map = L.map('map-container');

L.tileLayer('http://{s}.tile.osm.org/{z}/{x}/{y}.png', {
    attribution: '&copy; <a href="http://osm.org/copyright">OpenStreetMap</a> contributors'
}).addTo(map);

L.Routing.control({
    router: L.Routing.osrmv1({
        serviceUrl: `http://router.project-osrm.org/route/v1/`
    }),
    showAlternatives: true,
    lineOptions: {styles: [{color: '#242c81', weight: 7}]},
    fitSelectedRoutes: false,
    altLineOptions: {styles: [{color: '#ed6852', weight: 7}]},
    show: false,
    routeWhileDragging: true,
    waypoints: [
        L.latLng(57.74, 11.94),
        L.latLng(57.6792, 11.949)
    ]
}).addTo(map);
```

## Do you want any modification or report an issue?

This type definition is provided as a fundamental solution for configure and display a route by using leaflet routine machine. This definition may not be enough for advanced use cases  such as Interaction, Support for other routing machine back ends. If you need any support with such scenario feel free to contact me via [**talktochanaka@gmail.com**](mailto:talktochanaka@gmail.com).
