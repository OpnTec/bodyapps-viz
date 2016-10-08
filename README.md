[![Build Status](https://travis-ci.org/fossasia/bodyapps-viz.svg?branch=master)](https://travis-ci.org/fossasia/bodyapps-viz)
[![Join the chat at https://gitter.im/fossasia/bodyapps-android](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/fossasia/bodyapps?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

# BodyApps 3D Body Visualiser

3D body visualizer component for #bodyapps project

## About 
The Body Visualiser App is an attempt to create a web based 3D Human body visualiser with options to import body measurements , using Fashiontec’s BodyApps Web Service and model the human body using the slider functions.

The App supports the models for a Male , Female and a gender neutral Kids Body with options to modify following body measurements and features.

* Height
* Chest/Breast
* Neck Girth
* Neck Height 
* Shoulders
* Shoulder’s Slope
* Bust Girth
* Stomach Form
* Waist
* Arm Length
* Upper Arm Girth
* Wrist
* Hip Girth
* Hip Height
* Thigh Girth
* Lower Leg Length
* Calf

## Communication

Please join our communication channels.

Mailing List at: https://groups.google.com/forum/#!forum/bodyapps

Gitter chat at: https://gitter.im/fossasia/bodyapps

## Building the Project

1.Clone the Master Repo
2.Locate the folder , and run the index.html (Enable Javascript if not enabled)

## Folders
The project BodyViz has 3 folders
* css -Contains the style sheets for the BodyVisualiser
* models-Contains the .js files for the Human base models and their morph targets alongwith config files for all the models
* js-Contains three.js and UCSCharacter.js which allows to render and customize the models.

Along with this there are three other files 
* index.html - Visualises Male Body 
* female.html-Visualises Female Body
* kids.html-Visualises Kid’s Body


###  models
* skinned
* UCS
* basis.js-Three.js human male body model , exported by Blender
* female.js-Three.js  human female body model , exported by Blender
* child.js-Three.js  human kid body model , exported by Blender
* skins
* Highlighted_Muscles.jpg:Skin UV Map for the human body models.

* testconfig.json - config file for the male body.
* femaleconfig.json-config file for the female body.
* childconfig.json-config file for the kid’s body.

###js
* Orbit.js-Developed by three.js org , has functions to set up the camera orbits , and enable 3D toggle view.
* Three.js-Developed by three.js org , has functions to render the three.js exported models in web view and use Morph Targets to customise the human body Models
* data.gui.js-Developed by data.gui.js , allows to create sliders and gui for the visualiser.
* detector.js-Detects the windows resolution and adapts the visualiser’s resolution as per that
* UCSCharacter.js-Contains the functions to render call the model data and render it using three.js library.It also has functions to listen to the slider changes and update the body visualiser model as required.

## Additional Softwares and Libraries Used
### Three.js
Three.js is a lightweight cross-browser JavaScript library/API used to create and display animated 3D computer graphics on a Web browser. Three.js scripts may be used in conjunction with the HTML5 canvas element, SVG or WebGL. The source code is hosted in a repository on GitHub.

### Blender 2.70
Blender is an open source 3D application for modeling, animation, rendering, compositing, video editing and game creation. Blender is available for Linux, Mac OS X and Windows and has a large world-wide community.Blender can be used freely for any purpose, including commercial use and distribution. It's free and open-source software, released under the GNU GPL licence.

This project has extensively used Blender along with Three.js export/import script[1][2] , to design the morph targets and then export the models in three.js format.

### MakeHuman
MakeHuman is an open source 3D computer graphics software middleware designed for the prototyping of photo realistic humanoids. It is developed by a community of programmers, artists, academics interested in 3D modeling of characters.
MakeHuman is fully Open Source. The character output of MakeHuman is released to public domain under CC0, in order to be freely used in commercial and non-commercial projects. The database and the code are released under the GNU License Affero GPL.

MakeHuman models are used as the base models for this project and some morph targets have been developed taking inspiration from the morph targets of the MakeHuman Project.The MakeHuman project allows to export the models in various formats.
