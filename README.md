# BSc Thesis

![Banner Image](/doc/img/anatomy/all2.png)

**Title**: Near Real-Time Weather Rendering System \
**Author**: Matthias Thomann \
**Tutor**: Prof. Urs K&uuml;nzler \
**School**: BFH, Switzerland

## Abstract
Clouds contribute a substantial part to the overall ambience in games, but an implementation of such effects often proves to be more challenging than anticipated.
To get as close as possible to real clouds, this project engages in researching and developing a near real-time weather rendering system.
This means that real weather forecasts from **meteoblue** are used to visualize past, current and forecast weather at any given time of day.
The environment is created with elevation model data from **ArcGIS**. Live photographs from **Roundshot** cameras can be viewed side-by-side with the rendered output for comparison.

The document dives into the science of clouds and illustrates the ten distinct classifications and how each of those could be represented in a weather simulation. 
In order to achieve high fidelity, the implementation relies on concepts like Voronoi **noise generation** and **raymarching**, which means to generate a random 3D cloud pattern and render it in volumetrically.

At last, the goal of the project is to create a fully featured, near real-time weather rendering system in Unity.
It is able to render **procedural** and volumetric cloudscapes, for any given date and time.
An intuitive user interface allows the user to control the weather simulation manually or let it run automatically based on **meteoblue** weather reports.

The achieved solution shows great results and fulfills almost all specified requirements.
It is only missing the cirrus clouds, but features shadow casting and a rain **particle system**, which were both not originally planned.

For future work, the weather rendering system could be incorporated in a game or further improved to achieve even higher visual realism.

## Impressions

![Banner Image](/doc/img/results/wheel1.png)

![Banner Image](/doc/img/results/wheel2.png)

![Banner Image](/doc/img/results/wheel3.png)

![Banner Image](/doc/img/results/wheel4.png)

![Banner Image](/doc/img/results/wheel5.png)

![Banner Image](/doc/img/results/wheel6.png)
