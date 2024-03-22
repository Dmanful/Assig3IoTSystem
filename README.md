This assignment publishes data from multiple simulated environmental stations to Thingspeak via MQTT,
as well as reads the data from Thingspeak and visualizes data from specific environmental stations as well as specific sensor types.
There are three virtual sensor types: temperature (Celsius), humidity (%) and CO2 level (ppm)

You must have the following prerequisites installed before running the code.

Prerequisites:
Python 3
Jupyter (pip install jupyter)
Paho-mqtt library (pip install paho-mqtt)
Numpy library (pip install numpy)
MatPlotLib (pip install matplotlib)
Requests (pip install requests)

You must have
three thingspeak channels set up for each of the environmental stations, with fields for the three sensor types on each to run this
code as default, if you choose to modify the number of stations or sensors you will have to modify the corresponding fields in the code
(sensor_fields, sensor_titles, CHANNEL_IDS).


You must also change the MQTT client information (MQTT_CLIENT_ID, MQTT_USERNAME, MQTT_PASSWORD) as well as the Thingspeak 
channel info (CHANNEL_IDS, READ_API_KEYS) to that of your client and Thingspeak channels before executing the code. 

To execute the environmental station generation code:
1. Open the Jupyter Notebook ("jupyter notebook", navigate to the "Assignment 3 Generation.ipynb" file and open it
2. Run the code (Run All Cells)
3. The code will generate sensor data for 3 environmental stations, for 5.5 hours by default

To execute the station and sensor graph visualization code:
1. Open the Jupyter Notebook ("jupyter notebook", navigate to the "Assignment 3 Plotting.ipynb" file and open it
2. Run the code (Run All Cells)
3. The code will plot the sensor data from the last 5 hours for each station respectively, as well as plots for each individual
sensor type for all of the stations over the last 5 hours.

The generation code should be run before the visualization code. Visualization can be done with any amount of data, however it will only visualize the last 5 hours worth. 
