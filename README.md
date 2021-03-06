# MaterialFX
![splash image](https://github.com/cynex/MaterialFX/blob/master/MaterialFX/Resources/MaterialFX_Splash.jpg?raw=true)

[![YoutubeVideo](https://img.youtube.com/vi/ZZKjNVfgPjM/0.jpg)](https://www.youtube.com/watch?v=ZZKjNVfgPjM)

Material FX : A powerful free shader for unity.

Features:

- Subsurface Scattering
- Tessellation & Displacement
- Height map(Parallax effect)
- Rim Emission Effects
- Iridescence
- Reflection Probe Boosting
- Additional Cubemap Reflections
- FX Map(Growth, Snow, Wetness)
- Easy to use UI with included tools to repackage textures
- Standard Unity Shader Compliant (No LWRP, HDRP support as of yet)

Requirements:

- Unity, and a GPU with DX11 shader support (4.6 for Tessellation)

Download:

- Download repo for latest updates (beta)
- Download the unity package (https://github.com/cynex/MaterialFX/blob/master/MaterialFX/UnityPackage_MaterialFX.unitypackage?raw=true)

How to use:

- Install unity package or clone the repo into your project in Assets/MaterialFX
- Setup your object as usual, and select MaterialFX/MaterialFX from the Material shader list.
- Enjoy !

Workflow:

MaterialFX has a notable difference from the standard shader, and the first thing you'll notice is that the metallic map is called advanced PBR map. This is because we've taken the Metallic map (Smoothness on alpha) and also made use of the green and blue channels for curvature / thickness. You can repack these textures using the Repack functions built into the editor. You can get these Curvature / Thickness maps by baking your models from Substance Designer / Painter, or xNormal (free)

MaterialFX also uses another new texture called the Environment FXMap. This is a custom texture which is a mask layer for snow / growth / wetness areas. You can repack these textures from other maps to get a nice result using the repack functions included in the editor.


Planned revisions: (prior to Unity Asset store launch)
- Glass Shader
- Low Spec Variants
- Investigate LWRP, HDRP workflows for solution
