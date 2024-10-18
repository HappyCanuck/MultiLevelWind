# Plugin purpose
As the name implies, this OpenRocket plugin allows for different winds velocities and directions at various altitudes. 

# Change Summary
This fork updates the Java version needed to run the plugin with OpenRocket 23.09, but it should work also with version 22.02.
It also changes the baseline altitude levels to match FAA/NavCanada high altitude forecast reporting.
Finally, it corrects a bug where wind directions could not be read by OpenRocket within the 0°-90° range.

# Usage
Copy MultiLevelWindv23.jar to your OpenRocket plugin directory (`~/.openrocket/Plugins/` on Linux, `~/Library/Application Support/OpenRocket/Plugins/` on Mac, `...\Application Data\OpenRocket\ThrustCurves\Plugins\` on Windows), then restart OpenRocket.
You can add and configure it in the simulation edit dialog under Simulation options -> Add extension -> Flight -> MultiLevelWind

# Wind data sources
In Canada, high-altitude wind data can be obtained from the NavCanada website for a limited set of airports: https://plan.navcanada.ca/wxrecall/ (use the closest available airport to your launch site).
In the USA, consult https://aviationweather.gov/data/windtemp/ and again find the closest airport to your launch site.
You may need to convert the wind codes into readable format for the plugin.

# Compiling 
If you want to compile your own plugin version, all the *.java files are included in the repository.

## Many thanks to rocketsam2016 for creating and sharing the original work!
