# Export Guide

## First, Blender (2.70)

- Open `blank.blend`.
- Go to the rig.
- Delete everything except `None_Armature_Data` and `Pose`.
- Import the DAE model.
- Open its rig.
- Drag the model’s mesh onto the blank rig, then select **Object**.
- Delete the imported rig.
- Select the mesh → Wrench tab → assign the blank rig under **Object**.
- Save.

## Then, Latest Blender

- Go to **Material** tab, wait for load.
- Enable **Use Nodes**.
- Open **Shader Editor**.
- Add **Diffuse Image Texture** node.
- Connect `Color` → `Base Color`.
- Done.

## Exporting

- Export as **FBX** with embedded textures:
    - Set **Path Mode** to `Copy`
    - Click the **file icon** next to it
- Open exported FBX in Blender.
- Open rig, delete internal rig.
- Export again as FBX with embedded textures.

## Final

- Rig with Mixamo **60 FPS T-pose**.