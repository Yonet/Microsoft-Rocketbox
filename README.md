## MICROSOFT ROCKETBOX AVATAR LIBRARY
The Microsoft Rocketbox Avatar library consists of 115 characters and avatars fully rigged and with high definition that was developed over the course of 10 years. The diversity of the characters and the quality of the rigging together with a relatively low-poly meshes, makes this library the go-to asset among research laboratories worldwide from crowd simulation to real-time avatar embodiment and social Virtual Reality (VR). Ever since their launch, laboratories around the globe have been using the library and many of the lead authors in the VR community have extensively used these avatars during their research.


![AvatarsSample](MicrosoftRocketbox/docs/images/AvatarsSample.png?raw=true)

## Setup
The FixRocketboxMaxImport.cs script needs to go in “Assets/Editor”  in the Unity project. This will fix the import of the 3dsMax materials to Unity. I.e. Max materials assume that diffuse material was set by the texture, whereas Unity multiplies the texture colour with the flat colour. Second Unity's transparent  materials still show specular highlights and thus hair looks like glass sheets. The material mode "Fade" goes to full transparent. The import tool also selects  the highest resolution mesh as being activated by default.
By editing this file you might choose another poly level (they are "hipoly", "midpoly", "lowpoly" and "ultralowpoly") Or you could choose not to import by changing OnPreprocessMeshHierarchy.

The FixRocketboxMaxImport was contributed by Prof. Anthony Steed from University College London. 
 
## Running the sample

Import the desired avatar folder (including fbx files and textures of the avatar) to your unity project "Assets" folder.

Once the files are on the correct unity folders project you can open Unity and include the avatar to the scene.

## Contributors

Mar Gonzalez-Franco - Microsoft Research
Eyal Ofek - Microsoft Research
Markus Wojcik - Rocketbox (Original avatar creation team)
Dave Garagan - Havok
