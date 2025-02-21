# GeoCodeDemo

This repository contains a single-page web application that utilizes Leaflet to display a map and provides a textbox for users to input one or multiple placenames. Each line in the textbox is treated as a separate address, which is then geocoded using the Nominatim API from OpenStreetMap. Markers are added for each successfully geocoded address, and the map automatically fits the bounds to show all markers. Additionally, there is a button to download all marker locations as a GeoJSON file.

## Features

- **Leaflet Map:** Fullscreen interactive map using Leaflet with a tile layer from OpenStreetMap.
- **Batch Geocoding:** Users can enter multiple addresses (one per line) to geocode in a batch.
- **Marker Grouping:** All markers are added to a feature group to allow for proper handling and map view adjustments.
- **Zoom Control Positioning:** Custom positioning of the zoom control to the bottom right corner.
- **GeoJSON Download:** Ability to download the geocoded marker data as a GeoJSON file.
- **Responsive Design:** The application is designed to be fullscreen and adjust to different screen sizes.

## How to Use

1. **Open the index.html file:** This is a standalone file that contains all the required HTML, CSS, and JavaScript embedded.
2. **Enter addresses:** In the textbox at the top left, input one or more placenames (each on its own line).
3. **Geocode addresses:** Click the **Geocode** button to add markers to the map.
4. **View markers:** The map view will automatically adjust to fit all the markers.
5. **Download GeoJSON:** Once markers are displayed, click the **Download GeoJSON** button to save the locations in a GeoJSON file.

## Dependencies

This project uses CDN-hosted libraries:
- [Leaflet](https://leafletjs.com/) for mapping functionality.
- [Nominatim](https://nominatim.openstreetmap.org/) for geocoding.

## Usage Notes

- A 1-second delay is introduced between geocoding requests to comply with Nominatim's usage policy.
- The project is designed for users primarily in the United States, with the initial map view centered on the USA.

## License

This project is provided as-is, without any warranties. Check the license file for more details if applicable.

## Future Improvements

- Enhance error handling and user feedback for multiple geocoding errors.
- Allow customization of API endpoints for geocoding.
- Provide styling improvements and mobile responsiveness.

Happy mapping!