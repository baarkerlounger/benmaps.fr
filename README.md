# Forked from Ben Maps

[Web maps that don't track you](https://benmaps.fr)

## ![Screen shot](https://repository-images.githubusercontent.com/84752763/d3f2bc00-62d4-11e9-9c1a-d95bc8156386)

### Tech

- [React](https://facebook.github.io/react/)
- [Redux](http://redux.js.org/)
- [Mapbox GL JS](https://www.mapbox.com/mapbox-gl-js/api/)
- [Assembly.css](https://www.mapbox.com/assembly/)
- [Mapbox Geocoding API](https://www.mapbox.com/api-documentation/#geocoding)
- [Mapbox Directions API](https://www.mapbox.com/api-documentation/#directions)
- [Wikidata SDK](https://github.com/maxlath/wikidata-sdk)
- [Mapillary API](https://www.mapillary.com/)

This project was bootstrapped with [`create-react-app`](https://github.com/facebookincubator/create-react-app).

[Redux](http://redux.js.org/) to manage the state, with a middleware component (the [`api-caller`](https://github.com/benjamintd/mapbox-maps/tree/master/src/api-caller)) responsible for all the asynchronous calls.

[Assembly.css](https://www.mapbox.com/assembly/) for styling, which shrinks the main CSS code below 60 lines.

The search bar is a fork from [`react-geocoder`](https://github.com/mapbox/react-geocoder), with minor tweaks to be better integrated in the app. When available, additional POI information is retrieved from Wikidata (images, phone numbers, websites, etc.).

The directions are powered by the [Directions Traffic API](https://www.mapbox.com/api-documentation/#directions). It leverages anonymous data from millions of users to provide the freshest live traffic information, in order to route you around traffic and give you the best ETAs.

### Map Style and sprites

The sprites and glyphs are hosted on the Mapbox infrastructure.

### To run
Rename the `.env.sample` file to `.env` and add your Mapbox token and Mapillary Client ID

Then:

```
yarn
yarn build
yarn start
```
