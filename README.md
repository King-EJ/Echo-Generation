# Echo-Generation
VR mod for Echo Generation





ECHO GENERATION VR  v0.1.3 (test build) - Unity 6000.0.61f1, IL2CPP x64
=============================================

Install
-------
unzip to game folder, only tested with virtual desktop XR

**[Nefarius ViGEmBus](https://github.com/nefarius/ViGEmBus/releases) support - with the driver installed (ViGEmBusSetup_x64.msi in the zip) the VR
        controllers are a real virtual Xbox 360 controller ([Controls] InputMethod = Auto / ViGEm / InputSystem).**

The views - TAP R3 (right stick click) to switch
------------------------------------------------
THIRD PERSON (start) .. the game's own camera ([View] Follow = false), or following behind the player
                        ([View] Follow = true / VR menu "Third person: follow the player").
                        With the game's camera the right stick moves the game's camera like on a pad and
                        your view turns with it ([View] GameCameraRightStick).
                        
FIRST PERSON .......... you are at the player's head (head hidden); the player's arms follow your controllers.

Tap R3 = first <-> third person.  Hold R3 (0.5 s) = the game's own R3.

Battles stay in your view ([View] GameCameraInBattles2 = true puts them on the game's camera). The game's camera

scenes always use the game's camera ([View] GameCameraInScenes); your view comes back afterwards.

Battles in first person
-----------------------
  - HP floats over every fighter's head: party green, enemies red    [HandHud] HpBarsOverParty, HpBarsOverEnemies, HpBarSize
    (the game's own small bars are hidden then - they are drawn in the wrong place in VR)  [HandHud] HideGameHpBars
  - LEFT controller: the SP                                           [HandHud] LeftPanelPosition / LeftPanelWidth
    (the party cards are hidden; [HandHud] PartyCardsOnLeftHand = true puts them on the left hand too)
  - RIGHT controller: the skill menu and its description              [HandHud] RightPanelPosition / RightPanelWidth
  - RIGHT controller, beside it: the timed attack / block icon         [HandHud] TimedHitOnRightHand, TimedHitPosition, TimedHitWidth
  - choosing a target: the game's yellow triangle floats under that fighter's HP bar   [HandHud] TargetTriangleUnderHp
  VR menu -> "Battles (first person)".
The game's menus and HUD float on a screen in front of you.

Arms
----
First person: the player's hands follow your controllers (two-bone arm IK). [Arms] HandsFollowControllers,
InThirdPerson (third person too: the player's hands move like yours relative to your head).
Each hand can be moved / turned in the VR menu ("Hands").


Controls (the VR controllers are an Xbox pad)
--------
  triggers = LT / RT, grips = LB / RB, A B X Y, left stick = move, stick clicks = L3 / R3
  Right stick left / right ..... turn (first person / follow); moves the game's camera (game camera view)
  A + B together ............... Start
  X + Y together ............... Back
  Tap both stick clicks ........ re-centre the view
  Hold both stick clicks 1.2 s . VR settings menu (right stick = choose / change, A = select, B = close)

Disable: to disable Mod rename winhttp.dll to winhttp.dll.bak

[VR Mod Manager](https://github.com/King-EJ/VR-Mod-Manager/releases/tag/VRModManager)

LICENSES
-
Uses Astien's OpenXR bridge. Free, non-commercial.
