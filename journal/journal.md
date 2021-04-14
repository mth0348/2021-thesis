# Meeting protocol 

## \#01: February 22, 2021
### Formal and technical questions
* Repository? -> will be setup by tutor.
* Project specification? Should be analogous to project2 work. Topics should include:
    * What is the goal?
    * Was has been previously achieved?
* The expert's name is *Dr. Eric Dubuis* (not the same as the teacher)

### Meeting discussion
Gitlab repository [2021-BSc-weather-rendering-system](https://gitlab.ti.bfh.ch/cpvr-students/2021-bsc-weather-rendering-system) should be used as storage for all project files.

There should be two meetings with expert (may or may not include tutor):
* After the specification is written
    * Present what was achieved previously, present objective target
* At the end of the semester, before deadline is due.

**Documentation guidelines**
* Introductory chapter:
    * Results of previous work (include screenshots)
    * Sketch / estimate what is planned for thesis
* Lay out specific requirements, like UI params for weather system
* Meeting schedule (every Thursday, 2pm, starting 04.03.2021)
* Document to be finished by 19.03.2021 (draft to be submitted by 15.03.2021)

**Possible Topics**
* Performance optimization (compute shaders)
* Different layers of clouds (restrictive, only focus on important categories)
* Parameter-based system, render weather based on preset of data, interpolate between presets
* Realtime comparison
* Interview with meteoblue
    * If so, only do one
    * be serious, be informed
    * NEBIS school books as alternative literature (library in Biel)
* Check personal contacts, maybe someone knows about accurate realtime weather data
* Comaprison between real and rendered image would go beyond of scope
* MS Flight Simulator as source for comparison

**Tasks**
* Setup specification document
    * Lay out all topics, sum up, categorize, prioritize
    * Focus only on what makes sense for thesis
* Check out NVIDIA NSight debugger
* Setup meeting with meteoblue - How to extract cloud genera


Next meeting is scheduled for **March 4, 2021 at 2pm.**

**Time log**

| Task | time spent |
|----|---|
| Journal update | 2h |
| Setup of latex work environment | 1h |
| Initial draft of specification document | 4h |
| Compute shader research | 4h |
| Journal update | 1h |
| Planning update | 4h |
| Journal update | 2h |

Purchased Udemy course for learning compute shaders: https://www.udemy.com/home/my-courses/learning/

&nbsp;

&nbsp;
#
## \#02: March 04, 2021
### Formal and technical questions
1. How do I quote my own work?
2. Should I explain things that are already explained in project2?
3. MS Flight Simulator license? Gifting or paying in advance?
4. Cite Udemy course?
5. meteoblue interview idea:
    * (before interview: decide on types of clouds)
    * ask about most important types of clouds
    * talk about API and how data is processed for API
    * ask about how each property would influence cloud image
    * ask about "pictocode" property

**Answers to questions:**
1. a basic introduction to those topics is necessary, reference to project2 work, just mention previous work, citing is ok, reference is not necessary, but mention project2.
2. only if different, or based on previous work.
3. buy, spesen, herr gasenzer für spesen
4. cite udemy course, and section
5. bewölkungsgrad standard skala? 1/8 bewölkung
    * ask how pictocode is made
    * rainspot, what distance?
    * label as "technical meeting", not interview, but still call


### Meeting discussion
**Inputs from tutor:**
* Swiss Landestopographie data has been released, Luftbilddaten, Höhenmodelldaten, Geländedaten
    * Could be used to generate mesh, from topo grid
    * Orthographic photos can be used as textures
* PCs from lab can be used if performance is needed
* "Previous work" chapter in RS in chapter 2
* chapter testing: detailed testing for new features: like UI
* expert meeting
    * introduction (general overview, why/what is shader, basics)
    * technical dive ok, but not too deep

* final results:
    * printed version, including CD with source,
    * due: at defense

**Tasks**
* Next meeting is scheduled for **March 11, 2021 at 2pm.**

**Time log**

| Task | time spent |
|----|---|
|Documentation|8h|
|Documentation|4h|
|Documentation|4h|

&nbsp;

&nbsp;
#
## \#03: March 11, 2021
### Formal and technical questions
1. Mr. or Mrs. Gasenzer? Direct email address would help.
2. Sources of Swisstopo data?
3. swisstopo - I would like to include that, but should I define it as a mandatory or optional goal?

**Answers to questions:**
1. Mrs. Gasenzer
2. https://www.swisstopo.admin.ch/en/geodata.html
    * format openGIS reader, maybe converter from ESRI to FBX?
    * GeoTIFF images for swisstopo images: https://www.swisstopo.admin.ch/en/geodata/images/ortho/swissimage10.html

### Meeting discussion
* Mention meteoblue
* Mention roundshot

**Inputs from tutor:**
- ✅ prioritize
- ✅ outlook (what to do after)
- ✅ R.0 general knowledge about clouds / cloud formation
    - ✅ change over time?
- ✅ Mention meteoblue
- ✅ Mention roundshot
- ✅ add another point to meteoblue data, maybe fribourg?
- ✅ add graphic of noise (take from project2.pdf)
- ✅ blockdiagram -> high-level system model -> "weather system overview"
    - ✅ "Vision" topic is its own topic, before "scope of work"
    - ✅ "Weather Rendering System Vision"
        - ✅ diagram
            * more visual than UML, use images in diagram
        - ✅ descriptions
            * meteoblue
            * roundshot
            * swisstopo
            * shaders 
    - ✅ then "Scope of Work", starting with "Educational Objectives"
- ✅ gesamteindruck wichtiger als perfekte wolken
- ✅ "project maangement" too detailed ToC
- ✅ GRAPHICS ARE IMPORTANT!!!!
- ⬜️ (Empty box for later use, ignore this)

**Tasks**
* Submit draft of diagram over weekend of **March 13 + March 14, 2021.**
* Next milestone is to submit draft of project specification on **March 15, 2021.**
* Next meeting is scheduled for **March 18, 2021 at 2pm.**

**Time log**

| Task | time spent |
|----|---|
|Documentation|4h|
|Documentation|4h|
|Diagrams and graphics|4h|

&nbsp;

&nbsp;
#
## \#04: March 18, 2021
### Formal and technical questions
1. Will tutor be present at meeting tomorrow?

**Answers to questions:**
1. in the beginning, yes

### Meeting discussion
Next steps:
* Clouds + layers research
* prepare for meteoblue interview
* learn about compute shaders, continue Udemy course

**Inputs from tutor:**
* ✅ based on = "making use of additional compute shaders" or something
* ✅ "side-by-side view for visual comparison"
* ✅ system is not perfectly real-time, it's more "near real-time"
* ✅ add disclaimer for sentence above (data is downloaded in specific interval, prediction can be as base for interpolated data to get as close as real time)
    * scope of work - "real-time" abgrenzung
* ✅ real-life = "live weather"
* ✅ explain pictocode in a sentence
* ✅ ... some of the crucial variables "in the JSON file" are ...
* ✅ ~~move sentence "From all avaiable" to the format listing.~~
* ✅ "elevation model" instead of "height model"
* ✅ "real-life" = "live mode"
* ✅ "sandbox" = "play mode"
* ✅ Remove topic "future work"
* ✅ Visual testing
    * Comparison with roundshot photographs
    * Add test: reference MS Flight Simulator use for visual comparison
* ✅ "Performance optimization" = "rendering P O"
* ✅ Add "Available hardware" chapter 3.5
    * Personal PC 
    * Bei bedarf, machines in lab can be used
* ✅ R.2: "layers" = "characteristics"
* ✅ Alle requirements in eine tabelle "summary of requirements"
    * including a column "priority"
    * 3.2.2: mention that neural network would be necessary, omit in requirements
    * add "rendering performance optimization" to optional requirements
* ✅ "latency" oder "visual stutters"
* ✅ Progress evaluation milestone
* ✅ split "implementation" into three groups
    * data aggregation / processing
    * weather system
    * UI und roundshot images comparison
* ✅ "examination expert" = "thesis expert"
* ✅ firm = company
* ✅ "possibly arisen" = encountered
* ✅ final presentation: June 18, 2021
* ✅ arranged
    * Go through document and add glossary entries.
    * Write something to abbrv.
* ✅ add image to title page


**Tasks**
* Expert meeting is scheduled for **March 19, 2021 at 4pm.**
* Next meeting is scheduled for **March 25, 2021 at 2pm.**

**Time log**

| Task | time spent |
|----|---|
|Updated document|4h|
|Updated journal|2h|
|Updated graphics|4h|
|Updated document|4h|
|Spellchecked document|2h|
|Reviewd document|2h|
|Reworked requirements|3h|
|Added optional requriements|1h|

&nbsp;

&nbsp;
#
## \#05: March 19, 2021 - Expert meeting 1
### Formal and technical questions
**Agenda**
* Personal introduction
    * Me
    * Gelegenheit anbieten: Herr Dr. Dubuis
* Topic introduction
    * Previous Work
    * Fachbegriffe (noise, shader)
    * Vision
    * Goals
    * Planning
* Questions

**About me**
* Software Entwicklung, Web
* Mehrere Jahre interesse an Computergrafik, besonders in Zusammenhang mit Games
* Auch Grund für grafische Thesis
* Freizeit
    * Game entwickeln seit 3/4 Jahr
    * spiele selbst gerne Games

**Notes**
* Experte
    * Begeistert vom Thema
    * Simulation von lichtverteilung in geschlossener räume
    * meteo unterrichtet / wetter
* Fragte nach: flugwetterinformation: metar und taf
* Wolkentyp / Flugplatz gibt info raus an flugleitsystem
* Evtl auch Verifikation brauchen
* https://www.meteoschweiz.admin.ch/home/service-und-publikationen/beratung-und-service/flugwetter/metar-taf.html

* Aufgabenbeschreibung gilt! FUR IHN SEHR WICHTIG!
    * was heisst realistic?
        * define "realistic" in thesis report
        * what does it mean, how can we measure it?
        * doesnt have to be 2 pages long
        * is core result
        * "suitable methods" meaning?
        * "measure" similarity? meaning?

Bemerkungen:
* Wie wird Arbeit bewertet? 1/4
    * Bitte im Hinterkopf halten: implementation ist nur 1/4
    * rechtschreibung, english, citations, references correct, 
    * roter faden in der präsentation
        * scope first
            * what did i do during thesis
            * results
    * kein freipass: aber: er findet es besser, lieber mit betreuer kontakt aufnehemn und features streichen falls nötig, dafür alle teile der arbeit vernünftig abwickeln.
* genug früh termin für verteidigung
* genug früh termin für meeting 2

&nbsp;

&nbsp;
#
## \#06: March 25, 2021
### Formal and technical questions
1. swisstopo is not part of task description

**Answers to questions:**
1. .

### Meeting discussion
Next steps:
* Clouds + layers research
* prepare for meteoblue interview

**Inputs from tutor:**
* task description ist nicht verpflichtend
* statistisches Mass finden für auswertung
    * pixel-approach?
    * binarisation? -> pixel distribution -> "noise" image can be compared

**Tasks**
* via Email ok
* Next meeting is scheduled for **April 08, 2021 at 2pm.**

**Time log**

| Task | time spent |
|----|---|
|Weather front research|4h|
|Cloud types research|8h|

&nbsp;

&nbsp;
#
## \#07: April 08, 2021
### Formal and technical questions
1. .

**Answers to questions:**
1. .

### Meeting discussion
* Next: 
 * 

**Inputs from tutor:**
* describe "reverse engineer" method
* summary
 * strategy for implementation, how to proceed from that
 * maybe pseudo-code
 * interview moved 2-3 weeks
 * 3 cloud altitudes => 3 different layers => 3 shaders

**Tasks**
* Next meeting is scheduled for **April 15, 2021 at 2pm.**

**Time log**

| Task | time spent |
|----|---|
|cloud types|8h|
|Weather front chapter|4h|
|Warm weather front|4h|
|Cold weather front|2h|
|Occluded weather front|6h|
|Implementation approach|3h|
|ArcGIS integration|6h|

&nbsp;

&nbsp;
#
## \#07: April 08, 2021
### Formal and technical questions
1. Is ok not to use swisstopo buildings?
2. Is ok only to use ArcGIS plugin?
3. Find date for exam (between June 15 and July 8) - week of June 21st?
4. "As mentioned in the specification documentation" ok? (3.4)
5. FBM, Voronoi reuse. documentation?

**Answers to questions:**
1. .
2. .
3. .
4. .

### Meeting discussion
* other good source: https://melstrong.org/page-of-clouds/

**Inputs from tutor:**


**Tasks**
* Next meeting is scheduled for **April 22, 2021 at 2pm.**

**Time log**

| Task | time spent |
|----|---|
|implementation approach|12h|
|inkscape cloud graphics|4h|
|inkscape cloud graphics|4h|
|inkscape cloud graphics|4h|