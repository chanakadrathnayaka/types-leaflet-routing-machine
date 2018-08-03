## TypeScript definition for leaflet routing machine.js

Leaflet Routing Machine is an amazing plugin developed by [@perliedman](https://github.com/perliedman/leaflet-routing-machine) in order to draw routes on a leaflet map. TypeScript definition helps you to use this plugin in your typescript projects.

### How to use leaflet-routing-machine.js in an Angular 2+ project 

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
    ```TypeScript
        "styles": [
            "../node_modules/leaflet/dist/leaflet.css",
            "../node_modules/leaflet-routing-machine/dist/leaflet-routing-machine.css"
        ]
    ```
6. Import leaflet into the component
    - Add below import statements top of your component
    ```TypeScript
        import * as L from 'leaflet';
        import 'leaflet-routing-machine';
    ```
# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)


For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/chanakadrathnayaka/types-leaflet-routing-machine/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
