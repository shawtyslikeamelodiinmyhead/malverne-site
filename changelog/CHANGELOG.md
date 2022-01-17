## [8.0.0](#8.0.0)

### Added:

- Network optimizations everywhere
- Work in progress BCSO station
- Player connected/disconnected notification
- Fire Rescue uniforms
- More start menu view points
- Countdown before you can agree to the rules
- New ATM, Bank, Uniform Locker menus
  - Bank transfers enabled
- More car spawn pads at Leesburg car dealership
- Ability for law enforcement to issue citations
- Ability for civilians to pay citations at the Sheriff's Office (until courthouse is built)
- Electrical boxes on street light poles
  - They can be interacted with by select teams to make the lights flash red
- Ability to drag players when they are in handcuffs and place/take them out of vehicles
- More icons to speedometer hud to reflect locks, ignition, and engine
- Pay rates depending on rank, definitely temporary and will be adjusted
- Overhauled inventory system and abstracted it away from players, with new additions like:
  - A team gear locker menu (aka armory for BCSO)
  - Vehicle inventories
  - ... with frisking coming soon

### Changed:

- Major framework refactoring
- Grass, ground and tree leaves colors slightly lightened
- Road and sidewalk colors made slightly warmer tone
- All exterior doors now open outward due to Florida Building Code
- Increased amount of bullet hit particles spawned, with lots of blood coming out when you headshot/stab people
- Speedometer recolored white
- Meters like stamina, health, oxygen moved to bottom left of screen
- The toolbar now fades out rather than completely disappearing when tools are unavailable (in a car or menu)
- Experimenting with gunshot volume by distance
- The bottom row HUD with time/compass/version has been made larger
- Some buildings had windows in tight alleys, these windows have been removed
- Dropped items now disappear after a few minutes
- Increase pepper spray range

### Fixed:

- Fixed various tool bugs
- Fixed an issue with premature character loading
- Fixed item shop selection bug
- Fixed some bugs with accessories
- Fixed weather not affecting atmosphere density (fog)... it used to do this months ago but somehow I accidentally deleted the code
- Fixed the issue with deaths not triggering when standing still
- Car spawn pad checking
- Fixed issue with not being able to go through fire doors sometimes
- Doors to buildings now properly lock and close when the business is closed
- Radio now scrolls down when there is a new message
- Misc UI fixes

### Removed:

- 9MM ammo & gun removed from shop (as they have not been completed yet)

Keep in mind some particle and light effects may be bugged or delayed due to this: https://devforum.roblox.com/t/particles-beams-and-trails-all-disappearing-not-disappearing-when-supposed-to-and-causing-performance-issues/1584372/68

Data has also been reset

## [0.7.0](#0.7.0) (12/29/2021)

- Tool-related changes:
  - Added radar gun
  - Added pepper spray
  - Tools are now automatically equipped into a slot upon picking up. This means that you cannot pick up more tools that would fit in that
    slot, unless it is an "extra", of which you can hold 6 of (for now)
  - Some select tools and items now appear as visible accessories on the character, so you can tell if someone is armed for example. This also works with the toolbelts and holsters available in the game.
  - You can hold CTRL with a tool out in third person to look around
- UI-related changes:
  - Start menu converted to Roact with a new, fresh design that is a work in progress
  - Added a short intro logo sequence after you load in
  - Switched from Cmdr to Zircon for both commands and logging
  - Fixed bug where tool data would show when not equipped
- Misc:
  - Basic ammo box model added for item drops
  - Got rid of the lava in the second island town area, and filled it with trees for now, until it is developed.
  - Data reset

## [0.6.2](#0.6.2) (12/20/2021)

- New weapon stuff:
  - Weapons now easily usable in third person with a proper camera and control system
  - Basic reload animations added
  - Hit particles added (for surfaces and people)
- Knife perf optimization and improved hit detection.. still working on way to improve this
- Removed a lot of unnecessary prints from the client/server output so errors & warnings are more visible

## [0.6.1](#0.6.1) (10/26/2021)

- Shotgun has been added
- Shotgun ammo has been added
- New confirmation dialog UI for various purposes
- Swapped out some menu songs
- Misc bug fixes

## [0.6.0](#0.6.0) (10/20/2021)

- Converted most UI to Roact framework. Some changes as a result:
  - You can no longer despawn occupied cars
  - BCSO/BCFR fleet manager: Did away with the "sign in, sign out" system, you can now spawn or despawn any vehicle so long as it is not occupied, but it will show you who took out one that is spawned.
    - This was mostly done for simplicity reasons as well as compatibility with BCFR—before, for example, if the spawner of an ambulance left, the ambulance would disappear, leaving the rest of the crew stranded. This will no longer happen as it is attached to the team itself, not the player.
- Very basic gun framework is in. The Colby .45 has been added and can be purchased at the gun store in Leesburg.
- Updated knife hit detection
- Made night slightly brighter - Still experimenting
- Different notification sound for money-related events
- Fixed bug where rain would appear during transition to rainy weather before the clouds actually appeared
- You can now fall of the map and die without having to rejoin

## [0.5.3](#0.5.3) (7/24/2021)

- Rescripted car steering
  - Not reliant on FPS anymore, and should be more responsive also
  - Can also turn now when engine is off, just not when in park
  - The vaLues still could use tweaking, let me know!
- Auto-equip the keychain on spawn.
- Fixed some dynamic arm bugs

## [0.5.2](#0.5.2) (7/24/2021)

- Lessened gas depletion rate
- Lessened oxygen depletion rate
- Fixed bug where you would hear radio beeps with no radio
- Fixed bug where you couldn't stop honking

## [0.5.1](#0.5.1) (7/24/2021)

- Emergency lighting changes
  - Less reliant on FPS, should not slow down as much when your FPS drops.
  - Add alley lights
  - Fix surfacegui occlusion
  - Slight changes to flasher lightbar attahcments
  - Changes to ambulance pattern _-GlocksGaming_
- Convert status effect meters to roact, also new circular design
- Most keybinds will now act based on key down rather than key up, this change was made due to community suggestion
- Fixed radio not sending messages
- Fixed a button sound bug
- Convert admin notice hud to Roact
- Changed keychain key from L to R
- Removed blue color shift from night, orange morning color shift will remain

## [0.5.0](#0.5.0) (7/21/2021)

- Future lighting enabled, and the game's lighting has been adjusted to make it look better with this mode
- Some changes to emergency lights
  - Light sources positioned farther out to avoid large shadows
  - Window lights now look just like the outside light bars
- Added spawnitem command for admins
- Fixed some bugs
- Data reset

## [0.4.0](#0.4.0) (7/17/2021)

- Character arms and neck are now responsive and face the camera
  - Still working on the smoothing for other character's updates, it's a little wonky at the moment
- The mouse is now hidden and the camera is locked during use of any tool
  - Soon, the mouse will be hidden during ALL gameplay except when a popup menu is on your screen, because there will be no HUD that requires a mouse click.
- Vehicle windows are now breakable, this does not save for now
- Streetlight timing fixes
- Gas pump system should be more consistent

## [0.3.0](#0.3.0) (7/10/2021)

- 5 month hiatus. Sorry 😂
- Map changes:
  - Water level raised to better reflect the keys
  - Beach/park area added in corner of map
  - Warehouse added
  - Bridge to island #2 raised
  - Various lights added around buildings
- Notification sounds added
- Vehicle HUD changed to a speedometer
- Traffic lights
- Item shop framework + first item shop, the gun store
- New transitional randomized weather system.
- Other things I proobably forgot about over 5 months.....

## [0.2.6](#0.2.6) (2/12/2021)

- Changes to interaction system UX
  - There are now three states to an interaction: Hidden, Disabled, and Enabled
  - Hidden does not show. Disabled shows faded and red. Enabled shows normally and can be used.
  - This adjustment was made in hopes that new players will understand that they don't have access to some things, rather than think they are broken. Some interactions will still remain hidden to reduce clutter.
  - In the future, you will be able to interact with a disabled action to trigger an alternate function. For example, knocking on a locked door.
- Streetlights turn off a little later in the morning
- Added a deadzone for controller steering
- Headlights/reverse lights now emit a warmer white color

## [0.2.5](#0.2.5) (2/11/2021)

- Rounded the calculated gas price down to the nearest integer
  - We don't want decimal amounts in our economy, for simplicity
- Rounded up the gas price-it is now $2/u
- Minor rules/tos change
- Data reset

## [0.2.4](#0.2.4) (2/10/2021)

- Tool equipping, unequipping, and switching _should_ be a smoother experience now.
  - This could still be buggy so please mess with the tools a lot and check for errors.
  - I'm still working on getting the viewmodel to appear and disappear at the right time.
- Removed unused limbs from the knife animations, shouldn't be anything looking frozen anymore.
- Created a wide bounding box for dropped items
- Moved interaction positioning a little up
- Can no longer fuel by extremely miniscule amounts (for UX)
- Misc client code refactoring

## [0.2.3](#0.2.3) (2/8/2021)

- Patriot's third brake light moved to exterior
- Uncuff key logic has changed-rather than having to possess handcuffs, you simply must be clocked in BCSO.
  - This is ok because civilians will never have access to handcuffs, however they will have access to zipties which are one-time use.
- Job reception duplication fixed

## [0.2.2](#0.2.2) (2/8/2021)

- Added a business hours posting in all non-24hr registered buildings that reflects its opening and closing times. (all days are the same)
- Seats are back, and can be sat in via interaction
- Gun shop bound to business "Old Line Armory"
- More gun shop interior work
- Minor tuning to vehicle steering
- Locked various unfinished buildings
- Registered laundromat as a building
- Fixed a bug that caused not all items to drop on death
- Anchored some parts that were causing lag

## [0.2.1](#0.2.1) (2/7/2021)

- Misc bug fixes

## [0.2.0](#0.2.0) (2/7/2021)

- Knife, the first weapon
  - 3 attack animations
  - An equip sound, slash sounds, and hit sounds
  - Does damage when you hit a person, obviously. Pretty basic for now-hitreg may need to be improved.
  - (Upcoming features):
    - Breaking glass
    - Blood effects
- Vehicle chassis refactor
  - Torque and acceleration are now factored differently based on gear
  - Adjusted driving stats of all vehicles (WIP and untested-please provide feedback)
  - You can drive with keyboard whether you have a controlled plugged in or not
  - Fixed terragon's torque slope correction (It was backwards)
  - No longer needs to be unlocked while refueling
  - Readded hold-ignition to start the car
  - You can no longer turn the wheel while the car is off
- New interaction system
  - New design with a subject name above many interactions now, like "Vehicle" or "Door"
  - Display texts have all been changed to be more generic, like "Talk" or "Open" rather than "Bank Teller" or "Open Door"
  - Can now enter vehicles with a tool equipped (it will unequip as you enter. this could be buggy)
  - It now checks for obstructions between you and the object
    - For example, you cannot get in cars through walls.
    - This is bound to be buggy-let us know about any interactions that are hard to select.
  - Some keys have been switched around
  - (Upcoming features):
    - Controller support
- Terragon specific changes:
  - BCSO livery created
  - Third brake light moved to exterior
  - Raised suspension to make it look bigger (Sorry the model sucks)
- BCSO fleet changes
  - -Centurion #18
  - +Terragon #22
- Character addons such as BCSO's temporary belt and campaign hat now hide while in a vehicle
- Dealership default color changed (to encourage players to try colors other than black)
- Adjusted permissions for various interactions
- Fixed start menu music randomly breaking
- All chairs have been temporarily disabled
- Data reset

## [0.1.4](#0.1.4) (1/26/2021)

- Recoded oxygen logic-should be able to float safely now.

## [0.1.3](#0.1.3) (1/25/2021)

- Removed some unimplemented items
- Added donator symbol in playerlist
- Fixed some broken doors
- Adjusted footstep volume
- Misc bug fixes and improvements

## [0.1.2](#0.1.2) (1/22/2021)

- Vehicle fx and huds should now update properly
- Made the watermark slighty less visible

## [0.1.1](#0.1.1) (1/21/2021)

- Fixed gas refueling
- Fixed loud radio sound when you join
- Added sound when you start transmitting
- Increased airhorn volume again
- Tree leaves now non-collidable

## [0.1.0](#0.1.0) (1/21/2021)

- Vehicle gas!
  - Added a gas cap to all vehicles except ambulance (will be added in patch)
  - Drains based on gear and speed.
  - It can be filled up at the gas station pumps.
    - Park outside the pump, turn the engine off, get out, and walk up to the pump.
    - As of now you can only fill the tank using all of your available cash.
    - The gas station will be remodeled soon.
  - When empty, your vehicle will turn off.
  - It saves with your vehicle.
  - Vehicles ordered by smallest to largest tank:
    - Centurion, Patriot, Terragon, Ambulance
- (Temporarily) removed vehicle ignition-hold
- Optimized some vehicle code
- Starting time is now random
- Centralized random number sources
- Added error/warning icons in bottom right of HUD
  - When you see one of these, submit a bug report
- Changed inventory key from Period to G
- Slightly increased airhorn volume
- Adjusted badging color on Patriot
- Disabled skybox stars during rain
- Adjusted item & tool throttling
- Misc bug fixes and improvements
- Data reset

## [0.0.6](#0.0.6) (1/19/2021)

- Radio now only makes sound if message received on current frequency
- Fixed vehicle flip key
- Enable BCSO patches for recruits
- Slightly decreased ambulances steer rate

## [0.0.5](#0.0.5) (1/19/2021)

- Fixed tools not unequipping client-side when restrained
- Throttle/steer now disabled when chatting
- Fixed broken billboard code

## [0.0.4](#0.0.4) (1/19/2021)

- Fixed radio not showing up
- Started showing all nametags (temp)
- Added #players to pause menu
- Changed up some admin/staff perms

## [0.0.3](#0.0.3) (1/18/2021)

- Fixed pause icon showing when handcuffed
- Slightly refactored inventory code (stuff could have broke)
- Can now switch directly between tools
- Halved stamina depletion rate
- Fixed inaccessible doors on buildings unlocking during open hours
- Fixed watermark
- Misc bug fixes and improvements

## [0.0.2](#0.0.2) (1/18/2021)

- Normalized some sound volumes
- Fixed character glitches on spawn
- Added footstep sounds based on material
- Fixed admin notice hud
- Registered coffee shop as building
- Misc bug fixes and improvements

## [0.0.1](#0.0.1) (1/13/2021)

- Initial release
