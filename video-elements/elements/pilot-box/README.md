# Pilot Box
The `pilot-box` will render a nice expanding box animation with implants, boosters and their estimated cost.

## Example 
![example](assets/example.png)

## Example Animation
Note: Since it a GIF it as not as smooth as the import that will be in your video which will be 60 fps vs 30 fps of this give below. The speed of the animation is also slightly sped up due the converting from 60 to 30 fps.
![example](assets/example.gif)

## Adjustments
If you want to modify this component follow the instructions below.
1. Open up [Online Editor](https://editor.rive.app/) or [download](https://rive.app/downloads) the client 
2. Go to `Personal Files`
3. Drag the file `*.rev` to your workspace
4. Open up the new project
5. You can temporarily enable `Background (Hide Me)` or import a new background based on a image render of your video to get a feel for how the element will look in your scene. 
6. **Important** Always edit things on the `Design` tab to prevent ruining animations that are already setup for you.
7. Expand to tree on the left search for `Box Contents` → `{Augmentation Slot X}` in this element you will find a label to adjust the text and an image to adjust the icon. **note:** As this can be a bit tedious to edit, I will likely in time make a separate component to generate an image from text for the implant images & labels. 
8. Expand the tree on the left search for `Box Contents` → `Card Footer` → `Estimated Cost` → `{Cost}` to set the estimated cost.
9. Expand the tree on the left search for `Box Contents` → `Card Footer` → `{Date}` to set the date of the price check.

**Note:** If you need more room on the box, you can select the `Box` and adjust it downward. This won't affect the animation as it animates to 100% height.

## Positioning the Line
If you want to position the pointer and line precisely you can do so quite easily with the following instructions
1. First lets make sure we can see what we are doing, Find `Pointer` in the hierarchy and select it in the properties press the eye icon on the Clip segment. This ensures that the clip mask which is used for the animation is currently disabled.
2. Expand to tree on the left search for `Pointer` → `Pointer Circle` position this exactly where you want the animation to start.
3. Expand to tree on the left search for `Pointer` → `Line Top` → `Path` and press the `Edit Vertices` button.
4. You can now make the line be whatever you want. **note:** that if you need a lot more space and want a much longer line you'd need to expand the canvas and move the `ClipMask` further to the right.
5. Turn on the visibility which you disabled in step 1 to restore the animation.


## Fine tune content and animation based on your current video
1. Use your video editor software to create a render (image) of the moment you want to add the element.
2. Import this image into Rive by going to `Assets` → + and then add your file
3. Switch back to `Hierarchy`, right-click `Background (Hide Me)` and select `replace` then select your new image
4. You can now fine-tune the animation to match the scene composition

## Export
Once you made all the adjustments and want to add create the export of the animation to add to your video editor.

1. Be sure the `Background (Hide Me)` layer is hidden
2. Press the menu
3. Press `Open Render Queue`
4. In the new window select the tab `Queued`
5. And select the `+` icon
6. Switch mode to `Animation`
7. Format to `PNG Seq` and `60fps`
8. Press the ▶ button
9. Once this is done, go to the completed tab
10. Press ↓ button download the archive

## Import to video editor

1. Extract the archive in your video project folder, it will be a huge number of `png` images so extract them to their own folder.
2. In your video editor of choice add an `Image Sequence`

Each video editor is slightly different but generally you want these settings:
- `Use Original Size` to ensure the UX matches future elements you will also import to the video. 
- `Frame Rate` should be `60px`
