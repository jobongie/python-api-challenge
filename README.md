# python-api-challenge

## Weatherpy

randomly generated coordinates and found corresponding cities using citypy that seemed skewed towards **Jamestown, USA**

queried OpenWeatherMap for API data on city locations, printed each city byloop

put city, country, humidity, temp, lat, and long into **city_data** df

exports **city_data** to csv file **City_Data** to folder **output_data** 

removed cities with humidity at or above 100% varied between 6 and 16 cities, and put this into df **clean_city_data**

### PLOTS**
**Latitude vs. Temperature Plot**

"""This graph shows a general trend of higher temperatures closer 
to the equator, with declining temps as the latitudes move to 
the polar regions"""

**Latitude vs. Humidity Plot**

"""I don't see a trend that stands out here, the data really only
tells me that their are more cities that have a 60% to %80 relative 
humidity. If I had to guess I would say that correlates with most 
of worlds population living next to a body of water or where water 
is readily available."""

**Latitude vs. Cloudiness Plot**

"""The consistency of straight lines at the cloudiness %
at 0, 20, 40, 75, and 100 tells me a person looks outside and says
yeah today looks about this amount of cloudy and is thus a qualitative
value rather than a quantitative one."""

**Latitude vs. Wind Speed Plot**

"""Their are more cities in the northern hemishpere that are concentrated
around the lats of 20 40 and 60. They are also concentrated at wind speeds 
of around 5mph, suggesting that something moderates the wind speeds. I 
believe this suggests that their are more cities concentrated in the northern 
hemisphere and those cities are close to the ocean where breezes tend to be
consistent but of low speed."""

### Linear Regression**
**Northern Hemisphere - Max Temp vs. Latitude Linear Regression**
Saved in folder **images** under **north_temp_lat**

"""There is a direct correlation between latitude and temperature"""

**Southern Hemisphere - Max Temp vs. Latitude Linear Regression**
Saved in folder **images** under **north_temp_lat**

"""There is a direct correlation between latitude and temperature."""

**Northern Hemisphere - Humidity (%) vs. Latitude Linear Regression**
Saved in folder **images** under **north_hum_lat**

"""No correlation between latitude and humidity"""

**Southern Hemisphere - Humidity (%) vs. Latitude Linear Regression**
Saved in folder **images** under **south_hum_lat**

"""No correlation between latitude and humidity"""

**Northern Hemisphere - Cloudiness (%) vs. Latitude Linear Regression**
Saved in folder **images** under **north_cloud_lat**
"""No correlation between cloudiness and latitude"""

**Southern Hemisphere - Cloudiness (%) vs. Latitude Linear Regression**
Saved in folder **images** under **south_cloud_lat**

"""No correlation between cloudiness and latitude"""

**Northern Hemisphere - Wind Speed (mph) vs. Latitude Linear Regression**
Saved in folder **images** under **north_wind_lat**

"""no correlation between lattitude and wind speed"""

**Southern Hemisphere - Wind Speed (mph) vs. Latitude Linear Regression**
Saved in folder **images** under **south_wind_lat**

"""No correlation between latitude and wind speed"""




## Vacationpy

Import csv from Weatherpy output file **City_Data**

Added g-keys

Created heat_layer with gmaps using humidity as weight

Figure with heatlayer overlayed saved as png in **images** folder under **fig_vacationpy**

narrowed_city_df created based on conditions windspeed < 35, cloudiness <20%,
and temp between 60 and 75 degrees f

hotel_df created to find Hyatt hotels within a 5k radius of city using gmaps

Created marker_symbol layer overlayed on fig then saved in **images** folder under
the name **fig_2_vacationpy**
