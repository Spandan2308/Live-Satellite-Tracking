Here I have used the N2YO library to track live locations of various satellites. The library will fetch satellite data like TLE and positions using NORAD ID and the user's N2YO key. 

I have tracked five satellites: ISS, MALLIGYONG-1, ASTROSAT, CSS (TIANHE-1) and NOAA 20 (JPSS 1). Their live locations are then plotted on an earth map using Plotly (scatter_geo). 

The last block uses a leaflet-based folium library to track the constantly changing live locations of these satellites without reloading the map. However, given the limit to the number of transactions per hour by an user with N2YO API, the code is ineffective for constantly tracking satellites.    
