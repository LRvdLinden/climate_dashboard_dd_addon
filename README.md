<h1 align="center">Climate Dashboard - Dwains Dashboard Add-on (more_page)</h1> 


<p align="center">
  <a href="https://dwainscheeren.github.io/dwains-lovelace-dashboard/">
    <img src="https://img.shields.io/badge/Dwains%20Dashboard-Default-299ec2.svg" />
  </a>
  <a href="https://github.com/custom-components/hacs">
    <img src="https://img.shields.io/badge/HACS-Default-orange.svg" />
  </a>
  <a href="https://github.com/LRvdLinden/climate_dashboard_dd_addon">
    <img src="https://img.shields.io/github/v/release/LRvdLinden/climate_dashboard_dd_addon" />
  </a>
      <a href="https://github.com/LRvdLinden/climate_dashboard_dd_addon">
    <img src="https://img.shields.io/github/downloads/LRvdLinden/climate_dashboard_dd_addon/latest/total?color=purple&label=%20release%20Downloads" />
  </a>
    <a href="https://github.com/LRvdLinden/">
    <img src="https://img.shields.io/github/followers/LRvdLinden?style=social" />
  </a>
    </a>
    <a href="https://discord.gg/7yt64uX">
    <img src="https://img.shields.io/discord/688401603811999885" />
  </a>
</p>
<p align="center">Climate Dashboard in Home Assistant Dwains Dashboard.</p>


<p align="center">Created by <a href="https://github.com/LRvdLinden">Léon van der Linden</a>
</p> 


<p align="center">
  <img src="https://user-images.githubusercontent.com/77990847/115149631-4124bd80-a065-11eb-98aa-f2694cbdcb79.png" />
</p>


## Prerequisite
---
- Make sure you have installed the lovelace [mini-graph-card](https://github.com/kalkih/mini-graph-card), [fontawesome icons](https://github.com/thomasloven/hass-fontawesome), and [Button Card](https://github.com/custom-cards/button-card). This can be done manually or directly via hacs.

<img width="618" alt="image" src="https://user-images.githubusercontent.com/77990847/114733529-b6ca1a00-9d43-11eb-876a-6f4beda466ec.png">



## Installation Add-on
---
- Copy the `climate_dashboard` folder in to the `dwains-dashboard/addons/more_page` directory.
- Open your `more_page.yaml` file in `dwains-dashboard/configs` and add the following;
```yaml
 - name: Climate Dashboard
   icon: mdi:home-thermometer-outline
   #main_menu: 'true' #Show this addon in the main navigation bar!
   path: 'dwains-dashboard/addons/more_page/climate_dashboard/page.yaml'
```
- Reload the theme configuration via Theme Settings

## Replace the following
---
- If some `sensors` not showing after this manual, please add the correct `sensor` to monitor
- If you want to refresh the dashbaodr every 10 minutes, add the following line to the `page.yaml` file
```yaml
 - cards:
   Refresh: null
   type: 'custom:auto-reload-card'
   delay_in_minute: 10
```

## Result
---
<img width="1262" alt="image" src="https://user-images.githubusercontent.com/77990847/115149558-fc008b80-a064-11eb-9066-c40e01d7e808.png">
<img width="1251" alt="image" src="https://user-images.githubusercontent.com/77990847/115149623-39fdaf80-a065-11eb-8bd2-39f335f5a888.png">




---
Enjoy my card? Help me out for a couple of :beers: or a :coffee:!

[![coffee](https://www.buymeacoffee.com/assets/img/custom_images/black_img.png)](https://www.buymeacoffee.com/LRvdLinden)
