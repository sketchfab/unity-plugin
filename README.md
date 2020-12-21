# Sketchfab Plugin for Unity

*Browse, import and export assets between Unity and Sketchfab*

*Based on khronos' [UnityGLTF plugin](https://github.com/KhronosGroup/UnityGLTF), the fork is available [here](https://github.com/sketchfab/UnityGLTF)*

This is a mirror repository for release only.

***Supported versions**: 2018+ (LTS) (2019 LTS is recommended as it uses the updated UI for which the plugin has been updated)*

A Sketchfab account is required for most of the plugin's features (you can [create one here](https://sketchfab.com/signup))


## Installation

Download the [latest release](https://github.com/sketchfab/unity-plugin/releases/latest) and import it like a regular Unity Package by double clicking on it. The plugin will be imported into your Unity Project inside `Asset/Sketchfab For Unity`.
**Please remove any existing Sketchfab plugin version before proceeding to avoid any conflict**

## Report an issue
If you have any issue, please visit [Report an issue](https://help.sketchfab.com/hc/en-us/requests/new?type=exporters&subject=Unity+Exporter) submit a support request.

A link is also available at the bottom right in the plugin interface.

## Sketchfab Asset Browser

**Available in menu: Sketchfab/Browse Sketchfab**

Browse, download, and import Sketchfab models directly into Unity editor.

You have access to:
 * more than 500k free downloadable models under Creative Commons licenses
 * models purchased on the [Sketchfab store](https://sketchfab.com/store/3d-models)
 * If you have a [Pro account or higher](https://sketchfab.com/plans), you also have private access to all the models published on your Sketchfab account, without requiring them to be downloadable to other users.

#### Authentication

*You need a Sketchfab account to download and import models from Sketchfab*

*You need a paid Sketchfab account (**PRO or higher**) to have a private access to your own models for download and import*

#### Asset Browser UI

Browse free Sketchfab downloadable models from the plugin using search and filters.

![browser_2](https://user-images.githubusercontent.com/4066133/102769855-8240e580-4383-11eb-84f9-8914c6a52abc.jpg)

Click on a thumbnail to show the corresponding model page with a button to download and import the asset

![modelview_down1](https://user-images.githubusercontent.com/4066133/102770065-cd5af880-4383-11eb-864c-2d39b51a3e4d.jpg)

##### Import options

The model will be imported in your project directory and merged into a prefab.

You can choose where to import the data in your project by setting **Import into** option. This parameter is set to `Assets/Import/{model_name}` by default (as shown in the screenshot).

You can also specify a **Prefab name** for this model, and also choose to **instianciate the model in your scene** immediately after the import.

Click the "Download model" button to start the operation which will first download the glTF asset of the model, and then import it into your Unity project.

![Imported](https://user-images.githubusercontent.com/4066133/102769900-9389f200-4383-11eb-905a-97be3be4a327.JPG)

## Sketchfab Exporter

*Available in menu: Sketchfab/Publish to Sketchfab*

Export and share your current Unity scene on Sketchfab.
*You need a Sketchfab account to download and import assets from Sketchfab*

Important note: glTF file format is used as transport between Unity and Sketchfab.

Because of this, a few features will not be supported and will be missing on the Sketchfab result.

The plugin will not export:
* animations or object handled by custom scripts
* custom materials/shaders

Only Standard materials (including Specular setup) are supported.

For animation, only Generic or Legacy animation type are exported.

![exporter_down1](https://user-images.githubusercontent.com/4066133/102770372-570ac600-4384-11eb-886c-e8caa79cc16b.JPG)

## glTF Importer (editor)

Small tool to import any local glTF asset into Unity
*Available in menu: Sketchfab/Import glTF*

Drag and drop glTF asset on the importer window, set the import options and click import.
![importer_down1](https://user-images.githubusercontent.com/4066133/102770731-e9ab6500-4384-11eb-91d2-84f7659e3234.JPG)
