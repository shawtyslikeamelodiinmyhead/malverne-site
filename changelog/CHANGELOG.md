## [0.13.1](#0.13.1) (3/27/2022)

### Fixed

- Fixed gas pump interaction
- Fixed being able to interact while in pickup truck bed

### Removed

- Disabled interaction sound for now until I can fix the flickering

## [0.13.0](#0.13.0) (3/27/2022)

### Added

- A couple new buildings have been added in Delfino
- A radio tower has been added to Vista Key
- Some map optimizations

### Changed

- Interaction system has been rewritten
  - It now allows you to interact with multiple objects' actions at the same time
  - If there are multiple interactions on screen with the same keybind, it will let you use the closest one
  - The interface is smaller
  - More performant as it uses new Roblox spatial queries
  - Some action names/subjects have been changed around
- Item/cash drops are no longer collidable with characters or vehicles
- Swapped many sounds to comply with Roblox audio privacy update
- Improved Centurion third brake light appearance
- Building numbers in windows have been converted to decals and will now disappear when the window is broken
- More windows across the map have been separated into different panes
- Due to the menu music being removed, you can now hear environment sounds in the start menu, so it's not dead silent
- Increased bloom size
- Refactored client weather transitions
- Moon and sun textures/sizes
- Circular meters are now hidden when in player menu
- Tourists now have access to the game

### Removed

- Menu music, for now

## [0.12.6](#0.12.6) (3/13/2022)

### Changed

- Moved flashlight from gun store to hardware store

### Fixed

- Fixed car inventory not saving

## [0.12.5](#0.12.5) (3/12/2022)

### Changed

- Slightly changed look of confirmation dialog box

### Fixed

- Fixed inability to use radio while sitting

## [0.12.4](#0.12.4) (3/11/2022)

### Fixed

- Fixed car spawning

## [0.12.3](#0.12.3) (3/11/2022)

### Added

- Some assorted perf optimizations

### Changed

- Chat is now disabled when not spawned in/alive
- Radio now moves down when chatting

### Fixed

- Fixed interactions not appearing properly with cars

## [0.12.2](#0.12.2) (3/9/2022)

### Changed

- Enlarged interaction hitbox for all doors
- You no longer lose stamina after jumping out of a seat

### Fixed

- Fixed issue with seats glitching you if you sit too fast after getting up
- Fixed interaction issue allowing you to sit in a seat through a window

## [0.12.1](#0.12.1) (3/8/2022)

### Changed

- The cage glass in the BCSO cage is now breakable

### Fixed

- Fixed more doors not opening/closing when supposed to
- Fixed ATAC/ammo not being purchasable in the gun store

### Removed

- Temporarily removed water wave changing as it's glitchy

## [0.12.0](#0.12.0) (3/8/2022)

### Added

- Added new pistol, Obeya FBW
  - 9mm ammunition
  - 15 round magazine
  - Weaker than Colby 45 (base damage 22)
  - Shoots faster than Colby 45
- Added new rifle, ATAC-786
  - 5.56x45 ammunition
  - 30 round magazine
  - Weaker than both pistols
  - Faster fire rate and more range and velocity than both pistols
- Added 3 new songs to menu music
- Added firearm chamber system
  - You can have magsize + 1 if you reload while there is a bullet in the chamber
  - There are different reloading animations based on whether there is a bullet in the chamber is full or not
  - Slide will now be affected by whether the chamber is empty or not
- Firearms now have a click sound if they are empty
- Added "Toggle ADS" game setting
- Moderation webhook for kicked users
- Added italian restaurant building (has dining room interior)
- Added lawfirm filler building
- Added ATM outside Delfino Used Cars

### Changed

- Changes to Colby 45:
  - Now does a little bit more damage (base damage 29)
  - Enlarged slightly
  - Now positioned relative to right leg when equipped without a holster
  - Re-animated
  - Re-colored/textured
- Changes to Colby CSG-12:
  - Re-animated
  - Re-colored/textured
  - Slightly increased fire-rate
  - Made it smaller
  - Changed fire sound
- Rescripted character extras (like bcso toolbelt), now can only be used if in team group
- Re-colored BCSO uniform extras (like stars/nameplate) to match badge color
- Sped up item shop transition
- Lessened rate limit for external records queries (players not ingame)
- Players who are sitting can now be handcuffed

### Fixed

- Fixed interaction bug causing keypresses to sometimes not do anything
- Fixed the logic that unlocks doors for businesses
- Fixed button sounds
- Fixed neon bleed from flashlight model
- Fixed player list not updating
- Fixed player menu "server uptime" showing player session time instead of the actual server uptime
- Some performance fixes

## Removed

- Removed 1 song from menu music

## [0.11.3](#0.11.3) (3/2/2022)

### Fixed

- Fixed not being able to arrest those employed with Cab Co
- Fixed issue with tool animations playing after unequipped
- Fixed long decimals in player menu weight bar
- Fixed civilian job cars not despawning after player left

## [0.11.2](#0.11.2) (3/2/2022)

### Added

- Added some more security measures to the game
- Gas cap to FR ambulance

### Changed

- Pepper spray now has more range, and now also depletes all stamina from the target
- Notification title and content has new line break
- Now only exterior doors will auto-close
- Slightly tightened spread on CSG-12

### Fixed

- Fixed wind ambience sound
- Fixed FR bay doors, again
- Fixed doors that should not have been unlocked
- Fixed some script errors from bug reports
- Fixed bug with pepper spray effects

### Removed

- Removed spawns in Delfino that are in the completely undeveloped part of the town

## [0.11.1](#0.11.1) (2/26/2022)

### Fixed

- Fixed FR bay doors

## [0.11.0](#0.11.0) (2/26/2022)

### Added

- The first civilian job!
  - Taxi company located in Delfino. This job is not automated (at least for now)—we recommend drivers collect payment with the drop cash feature before they take riders to their destination
  - It has a limit of the amount of players that can work for them at one time
  - Presence on civilian job "teams" will not persist between sessions
  - _Note: The taxi light is not functional yet. This will be patched in soon_
  - _Note: There will be a way to hand money to people rather than dropping it for everyone. This will be patched in soon_
- New notification design
- New "player menu" which is a combination of the old inventory menu and the pause menu from pre-alpha
  - Character tab
    - A view of your character's vitals, with room for more to come when the health system is expanded
    - A larger, more readable inventory menu
  - Settings tab
  - Controls tab, lets you view all of the game's key bindings, sorted by category (player, car, gun)
  - Server tab
    - Player list
    - Server uptime, player count, and game version
  - Over time, more of the UI will adopt this fullscreenish style, rather than the small menu boxes
- Client performance improvements
- Ability to surrender. You will not have access to your inventory while surrendered
- Ability to drop cash
- More shallow beach area in Leesburg
- Added SO/FR logos to their front doors

### Changed

- Salaries are no longer automatically deposited into your bank account. You must now manually collect them in cash at your place of work, or if it is civilian welfare, collect it from the county services building in Leesburg. Then you can go to the nearest bank and deposit it. The business/office will only hold up to $500 of payroll, and if the balance goes above that amount, you won't be paid (forces you to go collect payroll)
- Mouse is now hidden unless in a menu, and the camera now follows your mouse movements, Broadview plays more like other third-person games in this sense
  - If you need to move your mouse outside of the game, just press Alt+Tab like any other game
- Only some tools auto-rotate your character, like weapons
- Rules updated to version 2
- Clock and version hud made more visible
- Slightly changed water appearance
- Slightly adjusted sea/lake level
- Night has been made slightly brighter for playability reasons
- Weather probability tweaks
- Weather now slightly affects water wave size/speed
- Players that are being dragged now lose all controls
- Locked doors that shouldn't have been unlocked
- You can now only see if an item is department owned if you are apart of that department
- Changed Colby .45 sound
- Slightly randomized pitch for gun sounds

### Fixed

- Fixed transfer money dupe bug
- Fixed bugs with weather system
- Fixed color issue with terragon
- Fixed some issues with UI causing lag
- Fixed windshield citation interaction position
- Fixed bug with textbox input

Data has also been reset due to the money dupe issue

## [0.10.5](#0.10.5) (2/10/2022)

### Fixed

- Fixed issue with shops not working

## [0.10.4](#0.10.4) (2/10/2022)

### Fixed

- Fixed action bug caused by last patch

## [0.10.3](#0.10.3) (2/9/2022)

### Added

- Hank's Hardware building
- FLHSMV building (no interior yet)
- Some additional admin functionality
- Another song in menu music

### Fixed

- Fixed action bug that often occured with actions in close proximity (you no longer need to walk away for it to update)
- Fixed road decals overlapping messages

## [0.10.2](#0.10.2) (2/8/2022)

### Added

- Manual siren (V) for emergency cars

### Changed

- Airhorn/siren behavior for emergency cars

## [0.10.1](#0.10.1) (2/8/2022)

### Fixed

- Fixed some lag issues
- Misc bug fixes

## [0.10.0](#0.10.0) (2/7/2022)

### Added

- Law enforcement may now frisk people. Frisking is a quick action that can be done on a non-handcuffed person that simply tells you if they have a weapon.
- Law enforcement may now search people. Searching can be done on handcuffed individuals and brings up a full inventory display of that person, with the ability to, for now, drop the target's items onto the floor.
- New town on Coral Key off US 1, dubbed Delfino (Unfinished just like Leesburg so it has plenty of mock buildings)
  - Has a used car dealership where you can find cars for cheaper but in limited colors (other disadvantages to buying "used" will be added soon), as well as spawn cars
  - Has a dock (with a couple more coming soon)
  - More rural feel for this town
- Leesburg Used Cars rebranded to Leesburg Aerostar (Now only sells Aerostar cars), now has an interior
- A couple buildings now have interiors
- Ambulance car inventory can now be accessed through on the driver's side rear storage
- One more patrol car added to BCSO fleet

### Changed

- All road lines are no longer 3D and have been converted to decals directly ontop of the road
- Some of the county/town government pay has been adjusted
- BCSO uniform patch/badge refreshed
- Civilian spawn locations rearranged
- Broken glass now regen around 5 minutes after it is broken
- Opened doors now close around 30 seconds after they are opened
- Several building windows have been separated into multiple parts so that they can be individually broken
- All team-related actions have now been switched to the group. Now, the only use for "Clocking In" is getting paid, you can still access everything otherwise
- BCFR command car now uses same siren as ambulance
- The server will now always start at 12 PM, that way new players can get more oriented because most businesses will be open
- Patriots with a topper (Aka the BCFR command car) no longer have bed seating

### Fixed

- Some fences/poles that weren't collidable
- Cars (should) no longer move when getting in/out

## [0.9.1](#0.9.1) (1/26/2022)

### Fixed

- Fixed critical data error
- Fixed cash not being removed on arrest

Data has been reset

## [0.9.0](#0.9.0) (1/26/2022)

### Added:

- Players can now be booked and incarcerated by law enforcement
- Law enforcement can now perform a records query at a computer in their station
  - Includes citations, arrests, registered cars, and other miscellaneous info (as of now, cars are automatically registered when you buy them)
  - More computers in the BCSO station once we continue to model it, but you can use the booking computers for now

### Changed:

- Players with felonies can no longer purchase firearms from the legal gun stores, and must resort to other methods (TBA)
- Hardcoded a limit of 60 minutes for arrests and $1000 for citations, to prevent abuse (Experimental)
- Civilians are now paid $6 instead of $12

### Fixed:

- Miscellaneous item/tool related bugs

Data has also been reset

## [0.8.1](#0.8.1) (1/22/2022)

### Added:

- Flashlight/radio added to BCFR gear locker

### Changed:

- Most of the UI will now only render when it is in use rather than continuously

### Fixed:

- Fixed issue where you could get in your car right after pulling out a tool (_Thanks connor8033_)
- Fixed misc errors (_Thanks ii_PoliceLaws, Br1452232_)

## [0.8.0](#0.8.0) (1/22/2022)

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
- Ability for law enforcement to:
  - Issue citations
  - Handcuff, drag, and put/take players out of cars
  - Place detainees in holding cells
  - (BOOKING NOT IMPLEMENTED YET. WILL BE ADDED IN AN EMERGENCY PATCH. FOR NOW, LEAVE THEM IN THE HOLDING CELL FOR A FEW MINUTES.)
- Ability for civilians to pay citations at the Sheriff's Office (until courthouse is built)
- Electrical boxes on street light poles
  - They can be interacted with by select teams to make the lights flash red
- More icons to speedometer hud to reflect locks, ignition, and engine
- Pay rates depending on rank, definitely temporary and will be adjusted
- Gas can tool, which can be filled up at gas pumps and used to fill up car tanks
- Overhauled inventory system and abstracted it away from players, with new additions like:
  - A team gear locker menu (aka armory for BCSO)
  - Car inventories
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
- Car engines now only cold start on the first start
- Cars can now be exited while locked unless handcuffed
- Car locks can now be controlled by the front passenger

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
  - BCSO/BCFR fleet manager: Did away with the "sign in, sign out" system, you can now spawn or despawn any car so long as it is not occupied, but it will show you who took out one that is spawned.
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
- Car windows are now breakable, this does not save for now
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
- Car HUD changed to a speedometer
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
- Minor tuning to car steering
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
- Car chassis refactor
  - Torque and acceleration are now factored differently based on gear
  - Adjusted driving stats of all cars (WIP and untested-please provide feedback)
  - You can drive with keyboard whether you have a controlled plugged in or not
  - Fixed terragon's torque slope correction (It was backwards)
  - No longer needs to be unlocked while refueling
  - Readded hold-ignition to start the car
  - You can no longer turn the wheel while the car is off
- New interaction system
  - New design with a subject name above many interactions now, like "Car" or "Door"
  - Display texts have all been changed to be more generic, like "Talk" or "Open" rather than "Bank Teller" or "Open Door"
  - Can now enter cars with a tool equipped (it will unequip as you enter. this could be buggy)
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
- Character addons such as BCSO's temporary belt and campaign hat now hide while in a car
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

- Car fx and huds should now update properly
- Made the watermark slighty less visible

## [0.1.1](#0.1.1) (1/21/2021)

- Fixed gas refueling
- Fixed loud radio sound when you join
- Added sound when you start transmitting
- Increased airhorn volume again
- Tree leaves now non-collidable

## [0.1.0](#0.1.0) (1/21/2021)

- Car gas!
  - Added a gas cap to all cars except ambulance (will be added in patch)
  - Drains based on gear and speed.
  - It can be filled up at the gas station pumps.
    - Park outside the pump, turn the engine off, get out, and walk up to the pump.
    - As of now you can only fill the tank using all of your available cash.
    - The gas station will be remodeled soon.
  - When empty, your car will turn off.
  - It saves with your car.
  - Cars ordered by smallest to largest tank:
    - Centurion, Patriot, Terragon, Ambulance
- (Temporarily) removed car ignition-hold
- Optimized some car code
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
- Fixed car flip key
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
