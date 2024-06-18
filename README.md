<div align="center">
  <p>
    <a align="center" href="https://ultralytics.com/yolov5" target="_blank">
      <img width="auto" src="https://raw.githubusercontent.com/imcommonsense/MelVR/main/imgs/logo.png"></a>
  </p>
</div>

# ![Portal Stories: Mel icon by carl6005](imgs/icon.png "Portal Stories: Mel Icon by carl6005") Portal Stories: Mel VR
* THIS REPOSITORY MAY CONTAIN CONTENT OWNED BY [VALVE SOFTWARE](https://www.valvesoftware.com/) AND [PRISM GAME STUDIOS LTD.](prismstudios.org)
* ALL RIGHTS GO TO THEIR RESPECTIVE OWNERS
* Note: I'm back working on this mod! (patch? mod? guide? it's something or other!)

## Things that work
* 6DoF VR view
* Motion controls for portal gun and grabbable objects

## Things that need fixing
* [Everything that portal2vr needs fixed](https://github.com/Gistix/portal2vr#things-that-need-fixing)
* Use Portal Stories: Mel original Portal Gun
* Lights on Portal Gun do not line up with Portal Gun
* Prerendered cutscenes do not display correctly in headset.

## How to use
1. Navigate to your portal_stories directory ```steamapps\common\Portal Stories Mel\portal_stories``` and delete EVERY file that begins with ```pak01```
2. Download [MelVR.zip](https://github.com/imcommonsense/MelVR/releases) and extract the files to your Portal Stories: Mel directory (steamapps\common\Portal Stories Mel)
3. Disable "Allow background processing of Vulkan shaders" (Steam Settings -> Shader Pre-Caching)
4. Connect your headset, then launch Portal Stories: Mel with these launch options:
   
   ``` -insecure -window -novid +mat_motion_blur_percent_of_screen_max 0 +mat_queue_mode 0 +mat_vsync 0 +mat_grain_scale_override 0 -width 1280 -height 720 ```

4. At the menu, feel free to change [these video settings](https://imgur.com/a/blTSqk2).
5. Load into a chapter. 

## Troubleshooting
If you have no audio:
* Go to ```steamapps\common\Portal Stories Mel\portal_stories\maps``` and delete ```soundcache``` folder.
* Note: You may have to run the game once, then restart for the sound cache to fix itself.
  
If the game isn't loading in VR:
* Try opening SteamVR before the game
* Disable SteamVR theater in [Steam settings](https://external-preview.redd.it/1WdLExouo_YKhTGT6C5GGrOjeWO7qNdIdDRvIRBhw-0.png?auto=webp&s=0d4447a9d954e1ec15b2c010cf50eeabd51f4197)

If the game is stuttering, try: 
* Lowering video settings
* Lowering SteamVR Resoloution
* Please be aware that Mel VR <b>WILL</b> stutter in specific areas.

If the game is crashing, try:
* Lowering video settings
* Disabling all add-ons then verifying integrity of game files
* Re-installing the game

## Build instructions
1. ``` git clone --recurse-submodules https://github.com/lilliepad1/MelVR.git ```
2. Open l4d2vr.sln
3. Set to x86 Debug or Release
4. Build -> Build Solution

## Based on
* [portal2vr](https://github.com/Gistix/portal2vr)
  
## Utilizes code from
* [l4d2vr](https://github.com/sd805/l4d2vr)
* [VirtualFortress2](https://github.com/PinkMilkProductions/VirtualFortress2)
* [gmcl_openvr](https://github.com/Planimeter/gmcl_openvr/)
* [dxvk](https://github.com/TheIronWolfModding/dxvk/tree/vr-dx9-rel)
* [source-sdk-2013](https://github.com/ValveSoftware/source-sdk-2013/)

## Support the original developer! ([Gistix](https://github.com/Gistix))
<a href="https://www.paypal.com/donate/?business=YL7TGWKPCC9H8&no_recurring=0&currency_code=USD"><img src="https://pics.paypal.com/00/s/MDAwNDljNmUtZWZiZS00ZTI1LWFiMTMtZTdhZmQ5NmU5ZDUx/file.PNG" alt="Donate Button" style="width:auto;height:100px;"></a>

