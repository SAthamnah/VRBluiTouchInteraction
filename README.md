# VR Tablet with Blui (Touch Based Interaction)
This is an example project to help you integrate [Blui (WebBrowser Widget)](https://github.com/getnamo/BLUI-Unreal) with your VR project. We will use Blui in this example to create a VR tablet.

<img width="200" alt="image" src="https://cloud.githubusercontent.com/assets/1334174/5969395/201a1202-a7f1-11e4-98a4-12bc6793f830.png" />

This project is made on Unreal Engine 4.27.2

<img width="200" alt="image" src="https://github.com/user-attachments/assets/71c2db25-4e8a-4bee-9252-d1a47bf6b237" />

___
## Download Blui
1. Please first download the appropriate version of Blui for your Unreal Engine from [Here](https://github.com/getnamo/BLUI-Unreal/releases)

In our case its [v4.2.0](https://github.com/getnamo/BLUI-Unreal/releases/tag/4.2.0):

<img width="600" alt="image" src="https://github.com/user-attachments/assets/98cce2fd-cb6e-417f-b6ac-d82c7500212b" />

___
2. Then press here to start downloading the Plugin files

<img width="600" alt="image" src="https://github.com/user-attachments/assets/0d19901b-b08c-4226-a048-9a32396b5e45" />

___
3. Copy The Plugins folder to your Unreal VR project

<img width="500" alt="image" src="https://github.com/user-attachments/assets/7a6109ee-83bf-4d79-ac9d-176ecca5b25d" /> 
--> <img width="400" alt="image" src="https://github.com/user-attachments/assets/d422c27e-825f-4431-9367-749b5ae2fbf3" />

___
4. Open Project plugins and make sure the plugin is Enabled:

<img width="600" alt="image" src="https://github.com/user-attachments/assets/70c55c99-6cf8-47dd-b33d-f6e9c45704ff" />
<img width="600" alt="image" src="https://github.com/user-attachments/assets/431098bb-372b-4e15-b436-00a04e3971f6" />

___
## Test Blui

1. Press on the button in the corner of the content browser and then select BLUI Content

<img width="400" alt="image" src="https://github.com/user-attachments/assets/78d6aadf-83cd-4bf4-a03f-402720dfe6f7" />

___
2. Drag and drop "BluiWorldWidgetActorExample" to your scenes

<img width="600" alt="image" src="https://github.com/user-attachments/assets/c4d3754e-780a-454d-9393-b3ee78303478" />

___
3. Play from current camera position to test if the plugin runs correctly youtube should load on the widget

<img width="300" alt="image" src="https://github.com/user-attachments/assets/e6e961fe-e4a3-4b0d-898a-23b273fa28fa" />
<img width="600" alt="image" src="https://github.com/user-attachments/assets/814b6884-90b6-4c8c-9537-e85933055ecf" />

___
### Change URL to load
From the details tap you can change the URL to be loaded on the widget

<img width="200" alt="image" src="https://github.com/user-attachments/assets/f2d7dbc2-b4cf-4b7a-b5ed-710ad51f7969" />
<img width="600" alt="image" src="https://github.com/user-attachments/assets/43891bd5-6d52-41ce-8884-3465d5ad92b7" />

___
### Change Dimensions
If you select the widgit under the defualtsceneroot you can change the resoloution and rasio of the widget, EX 2000 by 1000:

<img width="200" alt="image" src="https://github.com/user-attachments/assets/44317aa6-abfd-44ec-b9a5-c0ea377d58df" />
<img width="600" alt="image" src="https://github.com/user-attachments/assets/61b8b920-9fd9-4f83-a737-b22b8ebd3553" />

___
## Touch Interaction in 3D space (VR Tablet)
### New Blui Widget in 3D space
1. Click on Add/Import in your Content Browser and create a new folder

<img width="300" alt="image" src="https://github.com/user-attachments/assets/cf8a99ca-7d8f-4d05-9588-5a434531c583" />

___
2. Open the new folder and Click on Add/Import again, press on Blueprint Class. Then select Actor and name it "VRTablet", open it by double clicking on it

<img width="300" alt="image" src="https://github.com/user-attachments/assets/87ad36dc-2090-4757-8bfc-c951ec02fc1d" />
<img width="300" alt="image" src="https://github.com/user-attachments/assets/d90124c8-a43d-400b-b959-b425f44e7fc3" />
<img width="300" alt="image" src="https://github.com/user-attachments/assets/cd28b1e5-164e-430a-bcc8-d1c0e5e8e51d" />

___
3. Press on Add Component and search for widget then click on it, Name it "screen". 

<img width="400" alt="image" src="https://github.com/user-attachments/assets/bf5f90c9-159c-4863-9bf8-641c4ebe039d" />

___
4. Under the details tap, Change the widget class to BluiWidget. You can view the widget from the Viewport tap.

<img width="300" alt="image" src="https://github.com/user-attachments/assets/a2718be5-d5f4-4b98-b730-4d41e32eb53c" />
<img width="500" alt="image" src="https://github.com/user-attachments/assets/4ca5cb5a-be87-4155-ad26-fef86b150361" />

___
5. Go back to the content browser and open "BluiWorldWidgetActorExample" right click on "InitBluiWidget" and copy the function, then go to your "VRTablet" Actor and right click on the functions section and paste the function.

<img width="400" alt="image" src="https://github.com/user-attachments/assets/9c70f904-59dd-461f-9e42-bed9b3138b25" />
<img width="236" alt="image" src="https://github.com/user-attachments/assets/611951af-f4cd-4553-8152-f3f1c3a4f616" />
<img width="352" alt="image" src="https://github.com/user-attachments/assets/000f2b27-ef5f-49dd-a768-ee2b217dd327" />

___
6. Open the function and drag and drop the screen component to replace the widget component. Right click on each missing variable then press create. Compile.

<img width="500" alt="image" src="https://github.com/user-attachments/assets/b85172a3-e63c-4c6c-8baf-845061c8d7b9" />
<img width="500" alt="image" src="https://github.com/user-attachments/assets/1342158c-acb7-4aa2-925f-6fadb7526930" />
<img width="300" alt="image" src="https://github.com/user-attachments/assets/c98b7a1a-c8c0-4287-ac36-0bd829790862" />

___
7. Open the Event Graph, Right click in the empty space, search for "initBluiWidget" and add it to your graph. Then connect it with "Event BeginPlay" then hit compile.

<img width="500" alt="image" src="https://github.com/user-attachments/assets/dac27ffd-25fd-4405-990d-f7639c9ea5c9" />
<img width="500" alt="image" src="https://github.com/user-attachments/assets/b5237355-69c9-4502-adc4-1733deb3f8d3" />

___
8. Change the default value of the URL variable to any website you want by clicking on the variable and writing the URL in the details tap.
<img width="700" alt="image" src="https://github.com/user-attachments/assets/f5a8e371-3159-4fdc-b9fc-0f77ce2ecbc0" />

___
If you drag and drop the current "VRTablet" to the scene it will look like this

<img width="700" alt="image" src="https://github.com/user-attachments/assets/fd180dfd-9112-4194-a46c-b5feb6cbb2c2" />

___
9. To fix the rendering change the screen Draw size to something semilar to a real tablet (1920,1080), then scale it down in your scene.

<img width="700" alt="image" src="https://github.com/user-attachments/assets/697bcd1f-27ac-4ccd-97e2-b8e5a4d23185" />
<img width="700" alt="image" src="https://github.com/user-attachments/assets/a9cf6a40-f7c0-4d76-a8d7-b863ecd87b82" />

___
10. Go back to your "VRTablet" Actor and add a new cube component, name it "Body". Unlock the scale and agust it to the appropriate size. Move the "Body" back to make the screen appear on the surface.

<img width="200" alt="image" src="https://github.com/user-attachments/assets/65e5b010-5b55-4676-9d1e-45ef5dc6e0b2" />
<img width="600" alt="image" src="https://github.com/user-attachments/assets/41d93819-c9e6-408c-9927-87268612316a" />
<img width="600" alt="image" src="https://github.com/user-attachments/assets/b813e115-04f7-4c76-991b-422458819d65" />
<img width="400" alt="image" src="https://github.com/user-attachments/assets/9eb1eac6-16a5-4d70-beda-2c093fd62852" />

___
### Touch Interaction






MIT License
