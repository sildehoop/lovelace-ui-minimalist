# My Home Assistant
At the top of each page we find the [chips](#chips) which allow me to quickly visualize the important information of the page.
Then [title](#title) to separate the different sections
and [cards](#cards) to represent and interact with devices, sensors, etc …
I used the custom component [button-card](https://github.com/custom-cards/button-card) for all these cards.
I drew a lot of inspiration from [7ahang’s work](https://www.behance.net/gallery/88433905/Redesign-Smart-Home) that I found on Behance.

<img src="https://user-images.githubusercontent.com/12232620/127769479-a8d2a117-7c1d-49f1-a8a2-6e3d51a4672c.png" width="200"><img src="https://user-images.githubusercontent.com/12232620/127769475-01b39e04-065f-4ea4-adb0-39bc5e9aa39c.png" width="200"><img src="https://user-images.githubusercontent.com/12232620/127769477-4010a487-927f-479a-8596-2bf19a9a4299.png" width="200"><img src="https://user-images.githubusercontent.com/12232620/127769478-229d04d9-db00-4b78-b14b-dcd91f7ff463.png" width="200">



## Table of Contents
- [Installation](#installation)
- [Design system](#design-system)
- [Chips](#chips)
- [Scene](#scene)
- [Title](#title)
- [Cards](#cards)

# Installation
1. Add **button_card_templates** in **ui-lovelace.yaml** file. 
    ```yaml
    button_card_templates: !include lovelace/button_card_templates/button_card_templates.yaml
    ```
4. Add **resources** in your **configuration.yaml** file. You will need at least [button-card](https://github.com/custom-cards/button-card)
    ```yaml
    lovelace:
      mode: yaml
      resources: !include lovelace/resources/resources.yaml
    ```
3. Add **themes** in your **configuration.yaml** file
    ```yaml
    frontend: 
      themes: !include configuration/themes.yaml
    ```


# Design system
## Colors
I tried to set up a consistency between the colors used to represent the entities.
<table>
<tr>
<th> Color </th>
<th> Type </th>
</tr>
<tr>
<td>

![orange](https://user-images.githubusercontent.com/12232620/127771417-73385ee2-8c31-47a4-8438-472826184ea1.png)

</td>

<td>
💡 Light
  
⚡ Electricity
</td>
</tr>
<tr>
<td>

![red](https://user-images.githubusercontent.com/12232620/127771470-38b1eba2-fc8a-41a8-a1fa-5fa249619af6.png)


</td>
<td>

🔥 Heating

</td>
</tr>
<tr>
<td>

![Blue](https://user-images.githubusercontent.com/12232620/127771485-615cf15e-d7fe-4528-8ccb-db3c307c3428.png)


</td>
<td>
  
☑️ On/off devices
  
🏠 Home
  
</td>
</tr>
<tr>
<td>

![green](https://user-images.githubusercontent.com/12232620/127771492-1abcd92b-8261-45e6-bdfb-d7987dcb6c76.png)


</td>
<td>
  
🌲 Exterior
  
</td>
</tr>
</table>


# Chips
![Chips](https://raw.githubusercontent.com/TBens/lovelace-ui-minimalist/main/screenshots/chips.png)
<details><summary>Code template</summary>
<table>
<tr>
<th> Template </th>
</tr>
<tr>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates/chips/chips.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
</tr>
</table>
</details>

## Temperature
![Chips - Temperature](https://raw.githubusercontent.com/TBens/lovelace-ui-minimalist/main/screenshots/chips_temperature.png)
<details><summary>Code</summary>
<table>
<tr>
<th> Example </th>
<th> Template </th>
</tr>
<tr>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates_examples/chips/chips_temperature.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates/chips/chips_temperature.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
</tr>
</table>
</details>

## Electric consumption
![Chips - consumption](https://raw.githubusercontent.com/TBens/lovelace-ui-minimalist/main/screenshots/power_consumption.png)
<details><summary>Code</summary>
<table>
<tr>
<th> Example </th>
<th> Template </th>
</tr>
<tr>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates_examples/chips/chips_power_consumption.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates/chips/chips_power_consumption.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
<td VALIGN=TOP>
</tr>
</table>
</details>

## Presence counter
![Chips - Present](https://raw.githubusercontent.com/TBens/lovelace-ui-minimalist/main/screenshots/chips_location_present.png)
<details><summary>Code</summary>
<table>
<tr>
<th> Example </th>
<th> Template </th>
</tr>
<tr>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates_examples/chips/chips_location_present.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates/chips/chips_location_present.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
</tr>
</table>
</details>

## Return button
![Chips - return](https://raw.githubusercontent.com/TBens/lovelace-ui-minimalist/main/screenshots/chips_return.png)

<details><summary>Code</summary>
<table>
<tr>
<th> Example </th>
<th> Template </th>
</tr>
<tr>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates_examples/chips/chips_return.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates/chips/chips_return.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
</tr>
</table>
</details>

# Scene
![Scene](https://user-images.githubusercontent.com/12232620/127768397-24ab76fc-b037-4fc5-a2ef-45e96285cd46.gif)
<details><summary>Code</summary>
<table>
<tr>
<th> Example </th>
<th> Template </th>
<th> Template Blue</th>
</tr>
<tr>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates_examples/scenes/scene.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates/scenes/scene.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates/scenes/scene_blue.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
</tr>
</table>
</details>

# Title
![Title](https://raw.githubusercontent.com/TBens/lovelace-ui-minimalist/main/screenshots/title.png)
<details><summary>Code</summary>
<table>
<tr>
<th> Example </th>
<th> Template </th>
</tr>
<tr>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates_examples/title.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates/title.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
</tr>
</table>
</details>

# Cards
![Cards](https://raw.githubusercontent.com/TBens/lovelace-ui-minimalist/main/screenshots/cards.png)

### Anatomy
![Anatomy](https://raw.githubusercontent.com/TBens/lovelace-ui-minimalist/main/screenshots/anatomy.png)
1. **Dot** : Visible when the device is unavailable. Also used on the entity **person**
2. **Icon** : Icon that represents the device
3. **Primary line** : Main information
4. **Secondary line** : Secondary information
5. **Optionnal part** : Possibility to display buttons to launch actions related to the device. Or display a graph to view the history of a sensor


## Light
![Light](https://raw.githubusercontent.com/TBens/lovelace-ui-minimalist/main/screenshots/light.png) 
<details><summary>Code</summary>
<table>
<tr>
<th> Example </th>
<th> Template </th>
</tr>
<tr>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates_examples/lights/light.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates/lights/light.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
</tr>
</table>
</details>

## Light slider
![Light-slider](https://raw.githubusercontent.com/TBens/lovelace-ui-minimalist/main/screenshots/light_slider.png) 
<details><summary>Code</summary>
<table>
<tr>
<th> Example </th>
<th> Template </th>
</tr>
<tr>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates_examples/lights/light_slider.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates/lights/light_slider.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
</tr>
</table>
</details>

## Outlet
![Prise](https://raw.githubusercontent.com/TBens/lovelace-ui-minimalist/main/screenshots/outlet.png)
<details><summary>Code</summary>
<table>
<tr>
<th> Example </th>
<th> Template </th>
</tr>
<tr>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates_examples/outlet.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates/outlet.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
</tr>
</table>
</details>

## Binary sensor
![Mouvements](https://raw.githubusercontent.com/TBens/lovelace-ui-minimalist/main/screenshots/binary_sensor-1.png) ![Fenêtres](https://raw.githubusercontent.com/TBens/lovelace-ui-minimalist/main/screenshots/binary_sensor-2.png)
<details><summary>Code</summary>
<table>
<tr>
<th> Example </th>
<th> Template </th>
</tr>
<tr>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates_examples/binary_sensor.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates/binary_sensor.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
</tr>
</table>
</details>

</td>
</tr>
</table>
</details>

## Door sensor
![Mouvements](https://raw.githubusercontent.com/TBens/lovelace-ui-minimalist/main/screenshots/binary_sensor-1.png) ![Fenêtres](https://raw.githubusercontent.com/TBens/lovelace-ui-minimalist/main/screenshots/binary_sensor-2.png)
<details><summary>Code</summary>
<table>
<tr>
<th> Example </th>
<th> Template </th>
</tr>
<tr>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates_examples/door.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates/door.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
</tr>
</table>
</details>

## Cover
![Volets](https://raw.githubusercontent.com/TBens/lovelace-ui-minimalist/main/screenshots/cover_buttons.png)
<details><summary>Code</summary>
<table>
<tr>
<th> Example </th>
<th> Template </th>
</tr>
<tr>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates_examples/cover.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
<td>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates/cover.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
</tr>
</table>
</details>

## Thermostat
![Thermostat](https://raw.githubusercontent.com/TBens/lovelace-ui-minimalist/main/screenshots/thermostat.png)
<details><summary>Code</summary>
<table>
<tr>
<th> Example </th>
<th> Template </th>
</tr>
<tr>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates_examples/thermostat.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates/thermostat.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
</tr>
</table>
</details>

## Water heater
![Chauffe-eau](https://raw.githubusercontent.com/TBens/lovelace-ui-minimalist/main/screenshots/water-heater.png)
<details><summary>Code</summary>
<table>
<tr>
<th> Example </th>
<th> Template </th>
</tr>
<tr>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates_examples/water_heater.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates/water_heater.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
</tr>
</table>
</details>

## Media player
![Enceintes](https://raw.githubusercontent.com/TBens/lovelace-ui-minimalist/main/screenshots/media.png)
<details><summary>Code</summary>
<table>
<tr>
<th> Example </th>
<th> Template </th>
</tr>
<tr>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates_examples/media.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates/media.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
</tr>
</table>
</details>

## Playstation
![Playstation](https://raw.githubusercontent.com/TBens/lovelace-ui-minimalist/main/screenshots/playstation.png)
<details><summary>Code</summary>
<table>
<tr>
<th> Example </th>
<th> Template </th>
</tr>
<tr>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates_examples/playstation.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates/playstation.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
</tr>
</table>
</details>

## Person
![Personne](https://raw.githubusercontent.com/TBens/lovelace-ui-minimalist/main/screenshots/person.png)
<details><summary>Information</summary>
    
**Dot** : 
- At home : Blue
- Away : Green 


**Dot icon** :
- At home : Home
- Away : Walking man
- Sleeping : Moon

**Comment** : The sleep state takes over the At home or Away state to display the moon icon
</details>
<details><summary>Code</summary>
<table>
<tr>
<th> Example </th>
<th> Template </th>
</tr>
<tr>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates_examples/person.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates/person.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
</tr>
</table>
</details>

## Generic
![Generic](https://raw.githubusercontent.com/TBens/lovelace-ui-minimalist/main/screenshots/generic.png)
<details><summary>Code</summary>
<table>
<tr>
<th> Example </th>
<th> Template </th>
</tr>
<tr>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates_examples/generic.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates/generic.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
</tr>
</table>
</details>

## Generic + graph
![Entity - graph](https://raw.githubusercontent.com/TBens/lovelace-ui-minimalist/main/screenshots/entity_graph.png)
<details><summary>Code</summary>
<table>
<tr>
<th> Example </th>
<th> Template </th>
</tr>
<tr>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates_examples/graph.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
<td VALIGN=TOP>

<!-- MARKDOWN-AUTO-DOCS:START (CODE:src=./lovelace/button_card_templates/graph.yaml) -->
<!-- MARKDOWN-AUTO-DOCS:END -->

</td>
</tr>
</table>
</details>
