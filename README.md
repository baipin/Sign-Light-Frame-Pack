# Sign-Light-Frame-Pack

Cities: Skylines II assets for a roadside sign light frame and a painted road-sign pole.

## Published assets

| Asset | Folder | Description |
|---|---|---|
| SignLight | [`assets/SignLight`](assets/SignLight) | Road-sign underlight and rear support frame. Matte painted support with a white lamp material. |
| StreetPole | [`assets/StreetPole`](assets/StreetPole) | 3 m road-sign pole with a light blue-gray matte painted finish. |

Both asset folders contain one main FBX and a `settings.json` file for automatic LOD generation. Import the whole asset folder into the Cities: Skylines II Asset Editor; do not combine files from different folders.

## Import workflow

1. Open the Cities: Skylines II Asset Editor.
2. Import the complete folder under `assets/SignLight` or `assets/StreetPole`.
3. Choose **Static Object / Prop**.
4. Keep the FBX filename and mesh name unchanged.
5. Let the editor read `settings.json`. If manual values are required, use LOD1 = 50% triangles and LOD2 = 20% triangles.
6. Click Import once and wait for processing to finish.

If an import is invisible, restart the Asset Editor and import only the selected asset folder. Do not add old test FBX files or extra external LOD files. An IOException mentioning `ImportedData` usually means a previous import still holds a Geometry cache file; close the editor, wait for the process to exit, then retry once.

## Source files

The `source` folder contains the Blender files used for the published assets. The exported FBX files are the files intended for the game editor.
