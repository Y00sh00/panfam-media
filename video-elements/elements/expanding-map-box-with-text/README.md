# Expanding Map Box with Text
The `expanding Map Box with Text` will render a nice expanding box animation to be used on-top of for example the EVE map.

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
6. **Important** Always edit things on the `Design` tab to prevent ruining animations that are already setup for you.
7. Expand to tree on the left search for `Box Contents` → `Title` → `{Text}` to update the title.
8. Expand to tree on the left search for `Box Contents` → `Title` → `Icon` to update the icon you can right click on it and replace it with another icon.

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

## Syncing the box with an animation
If you have a rotating or moving map and you want to keep the box in the same position

1. Pick a spot you want to anchor the image on that is easily identifiable in all frames for example a letter of a region on the map. 
2. Move the circle of the box to that spot
3. Now every second start making key frames and move this circle again to the right location.
4. Test your animation if it looks good you are done, if not also set key frames on half seconds.
