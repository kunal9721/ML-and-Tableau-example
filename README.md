Use case1: Cluster attached 4 vehicles basis the route taken by them and then generate insights like – Average Speed/Drive time/Fuel consumed and Total Trips taken by vehicles in that cluster.

Trip starts from: "SamaiPur, Delhi" to: "Chadarghat" or "Fursungi, Pune"

 

Use case2: Identify Hotspots where vehicle idles frequently and plot it onto map at both Vehicle level and Customer level.

Consider idling time>2 mins and minimum 4 instances to identify a Hotspot.

 

metadata of raw feed:

vin - vehicle chassis no(this is unique for every chassis)

latitude - Latitude of Vehicle location

longitude - Longitude of Vehicle location

altitude - Altitude of Vehicle location in meters

updateddate - is the event date or the occurrence of the event(i.e reflected in msg_trigger_type)

total_fuel_consumption - LOV(Life of vehicle) value of Fuel consumption(its cumulative value)

total_distance- LOV(Life of vehicle) of distance travelled (its cumulative value) by vehicle

time_idle - LOV(Life of vehicle) value of Idling time. Idling is when vehicle’s engine is ON but vehicle is stationary.

msg_trigger_type - are the various triggers on vehicle which cause a packet to generate. e.g. Ignition ON, Ignition Off, Periodic(after every 5 min), Periodic_with_Distance(after every 200mtr run of the vehicle) etc.
