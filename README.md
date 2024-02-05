# Mapping
pip install pandas geopy
import folium

def plot_location(latitude, longitude, zoom_start=10):
    # Create a map centered around the specified latitude and longitude
    map_location = folium.Map(location=[latitude, longitude], zoom_start=zoom_start)

    # Add a marker for the specified location
    folium.Marker([latitude, longitude], popup='Kolkata').add_to(map_location)

    # Display the map
    return map_location

# Coordinates for Kolkata
kolkata_latitude = 22.5726
kolkata_longitude = 88.3639

# Plot the location
plot_location(kolkata_latitude, kolkata_longitude)


import folium

# Latitude and Longitude for Jessore Road, Lake Town, Kolkata
latitude = 22.6000
longitude = 88.4000

def plot_location(latitude, longitude, zoom_start=8):
    # Create a map centered around the specified latitude and longitude
    map_location = folium.Map(location=[latitude, longitude], zoom_start=zoom_start)

    # Add a marker for the specified location
    folium.Marker([latitude, longitude], popup='Jessore Road, Lake Town, Kolkata').add_to(map_location)

    # Display the map
    return map_location

# Plot the location
plot_location(latitude, longitude)
