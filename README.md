# Hardware Integrations

## Lighting

![image](https://user-images.githubusercontent.com/6697133/117109100-c0bec600-ada1-11eb-804a-43ce45cdbacb.png)

### [Syska Smart LED Bulb](https://www.amazon.in/Syska-Compatible-Amazon-Google-Assistant/dp/B076JLQSSL/ref=sr_1_1?dchild=1&keywords=syska+rgb&qid=1619671253&sr=8-1)

Integration link - [Tuya](https://www.home-assistant.io/integrations/tuya)

A lot of cheap smart bulbs are essentially rebranded [Tuya](https://www.tuya.com/) bulbs. Which allows HA to then integrate with a "Syska" bulb. Unfortunately, there's no way to verify if your hardware will with on HA or not. It's a bit of a risk. Easiest way to check would be to search the Q&A and review section of the product and see if someone mentions using the Tuya app.

You'll have to fetch the Tuya app on your phone and configure the bulb using that. Once configured you can then install the integration on HA and follow the steps. 

### [Yeelight](https://www.amazon.in/Yeelight-Dimmable-Compatible-Assistant-Multi-Colored/dp/B07HYP72RS)

Integration link -  [Yeelight](https://www.home-assistant.io/integrations/yeelight/) 

Not much to add here. There's no workaround needed, works out of the box. I believe Yeelight is now branded as Mi Bulbs but the same integration might work. I cannot confirm as I don't have any Mi bulbs. 

### [Philips Wiz](https://www.amazon.in/Philips-Connected-Dimmable-Compatible-Assistant/dp/B07X922QQV/ref=sr_1_2?dchild=1&keywords=philips+wiz&qid=1619671774&sr=8-2)

Integration link - [wiz_light](https://github.com/sbidy/wiz_light).

Integrates through a custom integration that you have to install. Setup is straightforward after that. 

### [WLED](https://github.com/Aircoookie/WLED)

Integration link - [WLED](https://www.home-assistant.io/integrations/wled/)

I made a custom LED Strip that I stuck behind my monitor. You can find more details on my blog here - [Responsive Bias lighting with WLED](https://valmik.in/posts/bias-lighting-wled/). Setup is quite straightforward after that. 


## Media

### PS4

Integration link - [Sony Playstation 4](https://www.home-assistant.io/integrations/ps4/). This integration allows you to control the power state of the PS4. Along with that, you can also select which game you want to play from HA itself, which then turns on the PS4, and starts the game. 

![image](https://user-images.githubusercontent.com/6697133/117109237-fa8fcc80-ada1-11eb-967d-f323ced49e0f.png)

### Google Cast

Integration link - [Google Cast](https://www.home-assistant.io/integrations/cast/)

I have two Google Home Minis and one Chromecast Audio. They all work through this integration. 

### [Kodi](https://kodi.tv/)

Integration link - [Kodi](https://www.home-assistant.io/integrations/kodi/)

I have Raspberry Pi 4 that runs Kodi. I use this as my media player connected to my TV. 

---

## Displays

### Android Tablets

I have a Fire HD 10 and Lenovo Yoga 3 (that my friend graciously gave me). The Fire HD sits on my work desk and the Lenovo tab hangs on a wall in the kitchen. They both run [Fully Kiosk Browser](https://www.fully-kiosk.com/). Fully Kiosk also integrates with HA through a custom integration - [homeassistant-fullykiosk](https://github.com/cgarwood/homeassistant-fullykiosk). This allows me to do a bunch of things like - Control the screen, lock the tablet, monitor certain aspects like battery, wifi strength, etc. It also allows me to push any web page. Very useful in the kitchen! 

### Android App

My phone runs the [official HA app](https://play.google.com/store/apps/details?id=io.homeassistant.companion.android&hl=en_IN&gl=US). The app allows you to send a lot of interesting data back to HA. There's a lot of powerful automations you can make using this data, especialy geolocation based ones.

---

## Other

### [Broadlink RM Mini](https://www.amazon.in/Broadlink/dp/B08243KL64/ref=sr_1_1?dchild=1&keywords=broadlink+rm+mini&qid=1619672837&sr=8-1)

Integration link - [Broadlink](https://www.home-assistant.io/integrations/broadlink/)

This works in tandem with a custom integration [SmartIR](https://github.com/smartHomeHub/SmartIR) which makes it really easy to integrate existing TVs and ACs into HA. I currently only use this to control the AC in my bedroom. 

![image](https://user-images.githubusercontent.com/6697133/117109498-65d99e80-ada2-11eb-9123-7ee66d86a882.png)

![image](https://user-images.githubusercontent.com/6697133/117109578-81dd4000-ada2-11eb-9b36-879ab75cc566.png)

### [Octoprint](https://octoprint.org/)

Integration link - [Octoprint](https://www.home-assistant.io/integrations/octoprint/)

I have a [Creality Ender 3 v2](https://www.creality.com/goods-detail/ender-3-v2-3d-printer) FDM 3D Printer. Octoprint is a fantastic OSS project that allows you to remotely control and monitor your FDM 3D Printer. It also integrates with HA allowing me to monitor my prints from the HA dashboard and also create automations like notifying me when my print is finished. If you have a camera setup, you can also embed that feed into the dashboard using the [MJPEG Integration](https://www.home-assistant.io/integrations/mjpeg/).

### **Xiaomi Air Purifier**

Integration link - [Xiaomi Miio](https://www.home-assistant.io/integrations/xiaomi_miio/)

I have a air purifier in my bedroom. The HA integration allows me to control the fan setting for the purifier. Along with that the purifier has sensors for temperature, humidity and AQI that I fetch into HA to display on a dashboard. 

# Software Integrations

### Spotify

Integration link - [Spotify](https://www.home-assistant.io/integrations/spotify/)

Pretty straightforward integration. I use this integration to be able to control playback from any device that I can access the dashboard. This is useful when music is playing on speakers. This integration also allows you to browse Spotify from HA's UI and play media on any devices that you may have integrated

### Google Calendar

Integration link - [Google Calendar Event](https://www.home-assistant.io/integrations/calendar.google/)

I have specfic calenders that are connected to my account that I fetch data from and show in HA on the dashboard. This is great for my workspace tablet which allows me to quickly glance at meetings / events. 

### [AirVisual](https://api-docs.iqair.com/)

Integration link - [AirVisual](https://www.home-assistant.io/integrations/airvisual/)

This fetches AQI information that I feed to my dashboard for monitoring purposes. It's a good reference point when comparing with AQI in-house. 

### [Uptime Robot](https://uptimerobot.com/)

Integration link - [Uptime Robot](https://www.home-assistant.io/integrations/uptimerobot/)

Uptime Robot pings a certain IP / Domain every x number of minutes and monitors your services. It wouldn't make sense to self-host a monitoring service at home so I use a hosted service to fetch the uptime data and store it in HA which is then fed into my dashboard. 

### [System Monito](https://www.home-assistant.io/integrations/systemmonitor/)r

Integration link - [System Monitor](https://www.home-assistant.io/integrations/systemmonitor/) 

This pulls data from the system HA is installed on. For my setup I fetch the CPU Usage, and network in and out. This gives me a simple but useful way to monitor my server from the HA dashboard. 

#
