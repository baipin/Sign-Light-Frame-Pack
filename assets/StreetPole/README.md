# StreetPole

A 3 m Cities: Skylines II roadside sign pole with a light blue-gray sprayed-paint finish.

## Contents

- `StreetPole.fbx` – the only FBX to import
- `StreetPole_BaseColor.png` – 1024×1024 square Base Color texture
- `settings.json` – automatic LOD configuration

## Model and material data

- Mesh object: `StreetPole`
- Dimensions: `0.12 × 0.12 × 3.0 m`
- Base position: bottom at Z=0, object center at Z=1.5 m
- Material: `StreetPole_Painted`
- Finish: light blue-gray matte painted steel
- Metallic: `0.0`
- Roughness: `0.82`
- UV: Smart UV Project
- FBX axis: Forward `-Y`, Up `Z`
- FBX version: 7400 / FBX 2018

The `settings.json` file requests LOD1 at 50% and LOD2 at 20% of the source triangle count. The Asset Editor generates those LODs automatically; no external LOD FBX is included.

## Texture editing

Open `source/StreetPole_CS2.blend` in Blender, edit the `StreetPole_BaseColor` image in Texture Paint, save the PNG, and re-export `StreetPole.fbx` with the same object and material names. Keep the texture filename as `StreetPole_BaseColor.png` and keep it beside the FBX when importing.
