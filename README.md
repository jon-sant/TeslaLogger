# TeslaLogger

TeslaLogger is a self hosted data logger for your Tesla Model S/3/X/Y. Actually it supports RaspberryPi 3B, 3B+, 4B, Docker and Synology NAS.

# Configuration for Homeassistant
Due to file privilege issues and single file volume linking not working, some modificaitons were made to allow HA HASSOS portainer install to work.  Make sure you have samba installed in homeassistant.  Open samba to \\server\share.  Make folder 'mylogger'.  Download this repo zip from github.  Extract all files to \share\mylogger\.

Open portainer, add new stack and point to this github.

Wait a ~5 min for DB init, view teslalogger container logs.

## Enter your Tesla crendentials
Use your browser to go to:

http://raspberry/admin/password.php

Enter the same credentials as you use in your teslaaccount or app.

## Settings & Language
Available languages: English, German, Spanish, Italian, Norwegian, Nederlands, Portuguese and Russian - Translations are welcome

Change the language and units and reboot the Teslalogger.

http://raspberry/admin/settings.php

## Admin Panel
http://raspberry/admin/

## Grafana-Dashboard
http://raspberry:3000

Username: admin

Password: teslalogger

## Dashboard
http://raspberry/admin/dashboard.php

Customizing the Dashboard goes here: [LINK](dashboard.md)

## Fleet Statistics
Fleet Statistics can be used by anyone without Teslalogger. To compare your degradation and charging curves with the fleet, you need a Teslalogger.

### Degradation Statistics
https://teslalogger.de/degradation.php

### Charging Speed Statistics
https://teslalogger.de/charger.php

### Firmware Tracker
https://teslalogger.de/firmware.php

### Map of fast chargings by Teslalogger Users
http://teslalogger.de/map.php

## SSH for advanced users

Username: pi

Password: teslalogger

## Custom Points of Interest (POI)

Details how to add / manage your own Points of Interest (POI) are [described here](TeslaLogger/Geofence.md)

# German manual
http://teslalogger.de/handbuch.php

Translations are welcome :-)
Please contact us beforehand to allow a coordinated approach for translations.

# TeslaFi Import
You can import your TeslaFi data [here](TeslaFi-Import/README.md).

# Teslamate Import
You can import your Teslamate data [here](Teslamate-Import/README.md).

# Donations:
http://paypal.me/ChristianPogea

You can also use my referral code to buy a Tesla:
http://ts.la/christian7267

# Screenshots
 [Dashboard](dashboard.md)
![Image](https://raw.githubusercontent.com/bassmaster187/TeslaLogger/master/TeslaLogger/screenshots/Dashboard.PNG)

Grafana Dashboards: http://raspberry:3000
![Image](https://raw.githubusercontent.com/bassmaster187/TeslaLogger/master/TeslaLogger/screenshots/verbrauch_en.png)

![Image](https://raw.githubusercontent.com/bassmaster187/TeslaLogger/master/TeslaLogger/screenshots/trip_en.png)

![Image](https://raw.githubusercontent.com/bassmaster187/TeslaLogger/master/TeslaLogger/screenshots/laden_en.png)

![Image](https://raw.githubusercontent.com/bassmaster187/TeslaLogger/master/TeslaLogger/screenshots/ladehistorie_en.png)

![Image](https://raw.githubusercontent.com/bassmaster187/TeslaLogger/master/TeslaLogger/screenshots/ladestatistik_en.png)

![Image](https://raw.githubusercontent.com/bassmaster187/TeslaLogger/master/TeslaLogger/screenshots/akkutrips_en.png)

![Image](https://raw.githubusercontent.com/bassmaster187/TeslaLogger/master/TeslaLogger/screenshots/degradation_en.png)

![Image](https://raw.githubusercontent.com/bassmaster187/TeslaLogger/master/TeslaLogger/screenshots/SOCladestatistik_en.png)

![Image](https://raw.githubusercontent.com/bassmaster187/TeslaLogger/master/TeslaLogger/screenshots/vampirdrain_en.png)

![Image](https://raw.githubusercontent.com/bassmaster187/TeslaLogger/master/TeslaLogger/screenshots/vampirdrain_month_en.png)

![Image](https://raw.githubusercontent.com/bassmaster187/TeslaLogger/master/TeslaLogger/screenshots/visited.PNG)

![Image](https://raw.githubusercontent.com/bassmaster187/TeslaLogger/master/TeslaLogger/screenshots/Trip-Monatsstatistik.PNG)

![Image](https://raw.githubusercontent.com/bassmaster187/TeslaLogger/master/TeslaLogger/screenshots/geofence_edit.png)

![Image](https://raw.githubusercontent.com/bassmaster187/TeslaLogger/master/TeslaLogger/screenshots/timeline.png)

# Screenshots with ScanMyTesla integration #

![Image](https://raw.githubusercontent.com/bassmaster187/TeslaLogger/master/TeslaLogger/screenshots/Zellspannungen_ScanMyTesla.png)

![Image](https://raw.githubusercontent.com/bassmaster187/TeslaLogger/master/TeslaLogger/screenshots/HVAC-ScanMyTesla.png)

![Image](https://raw.githubusercontent.com/bassmaster187/TeslaLogger/master/TeslaLogger/screenshots/verbrauch-ScanMyTesla.png)

![Image](https://raw.githubusercontent.com/bassmaster187/TeslaLogger/master/TeslaLogger/screenshots/performance-ScanMyTesla.png)

![Image](https://raw.githubusercontent.com/bassmaster187/TeslaLogger/master/TeslaLogger/screenshots/Zelltemperaturen.PNG)

# Your Car vs Fleet #
![Image](https://raw.githubusercontent.com/bassmaster187/TeslaLogger/master/TeslaLogger/screenshots/MyDegradationVsFleet.PNG)
