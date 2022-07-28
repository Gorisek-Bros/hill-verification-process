Hill Approval Criteria
======================

Version: 1

Valid from: 2021-11-27

The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD", "SHOULD NOT", "RECOMMENDED",  "MAY", and "OPTIONAL" in this document are to be interpreted as described in RFC 2119 - https://datatracker.ietf.org/doc/html/rfc2119.

This document describes all criteria and guidelines that must be taken into consideration during verification of hill.

Rules marked as **[REAL]**, **[RETRO]** or **[FICTIONAL]** may be applied only to hills assigned to mentioned hill types in DSJ24.PL.

## I. General

1. Essential rules
    1. Hill must be uploaded to DSJ24.PL by its author.
    2. Hill must comply with DSJ24.PL Terms of Service.
    3. Only the latest uploaded version of hill may be subject of verification.
    4. Hill must be playable in the latest released DSJ4 version.
    5. Hill must not cause any game crashes or not intended changes to ski jumper during playing, including jumping from lowest or highest gates available in Training mode.
    6. Hill file size must not exceed 2MB.
    
2. Hill type
    1. Hill must be assigned to correct hill type available on DSJ24.PL.
    2. Hills of types DSJ2 REMAKE, DSJ3 REMAKE, and EXPERIMENTAL are not subject of Hill Approval Process and may not be approved.
    
3. Hill name
    1. Hill name must be a common place name where the hill is located. It may be a town, village, suburb or other locality name.
    2. **[RETRO]** In case if hill had more than one configuration or profile, its name must include year(s) when it was used.
    
4. Hill description and screenshots
    1. Uploaded hill must contain at least one screenshot with clearly visible inrun or downhill elements.
    2. Screenshots should not be edited in any way before uploading.
    3. Screenshots should be scaled to size 640x360.
    4. Hill description should contain a short information about the hill, its profile, location, or real-life hill records.


## II. Configuration, built-in elements

1. Hill author
    1. List of hill authors must contain all people who put significant effort to create the hill.
    
2. DSJ Version
    1. Hill must have set DSJ version to the highest value compatible with latest released game version.
    
3. Location
    1. **[REAL, RETRO]** Location of hill (latitude, longitude and latitude) must reflect real coordinates of the hill. Precise location can be determined by using external services, such as OpenStreetMap.
    2. **[FICTIONAL]** Hill must be based on location that exists in real life.
    3. Timezone must be set accordingly to country or region where the hill is located.
    
4. Weather
    1. Weather configuration should reflect conditions based on place where hill is located. Hill located in Northern Hemisphere (e.g. Central Europe) should have snow only during winter months.
    2. In most cases, default values should be used:\
        `pollution="0.0" firstsnow="300" lastsnow="90" maxsnow="1.5" precipitationprobability="0.1" fogprobability="0.1"`
    
5. Competition timing
    1. Hills that do not have any artificial lighting must have XML element Time set properly to ensure that no competitions will take place in darkness.
    
6. Flag
    1. Flag is a optional element of hill. It may be hidden by author. When hidden, following flag rules don't apply.
    2. Flag must be not too big. It should not fall down too much with strong wind (2.0 m/s).
    3. Flag should not pass through other visible elements of hill, excluding flag pole.
    4. Flag design must reflect country where hill is located.
    5. Flag must have correct proportions.
    6. Radius of flagpole should be proportional to its height and size of flag.
    
7. Downhill fence
    1. Downhill fence must be not too tall. It must not block view of ski jumper and downhill elements during jump.
    2. Downhill fence may be hidden by setting d0 attribute in element Fence or setting height to value lower or equal than 0.1.
    
8. Judgetower
    1. Hill should contain a visible judgetower.
    2. Judgetower must be connected with ground directly or through other construction elements.
    3. Default judgetower must be turned off if hill contains a custom one.
    4. Custom judgetower must be placed in exactly same place where the default judgetower would be placed.
    5. **[REAL, RETRO]** Custom judgetower, if present, must reflect appearance of the real tower.
    
9.  Custom cameras
    1. Custom startgate camera (F5) must be placed close to available startgates.
    2. Custom takeoff camera (F6) must be placed close to takeoff.
    3. **[REAL, RETRO]** Custom judgetower camera (F7) must be placed inside of judgetower, or outside of it if it will be used to resemble realistic TV camera view.
    4. Custom grandstand camera (F8) should be placed behind fall line of hill, inside or close to downhill zone.
    5. View from all custom cameras must be not blocked by any elements, such as fences, trees, or buildings.
    
10. Plastic
    1. Plastic color should be not too saturated, too bright, and too dark. It must not distract player during jump.
    2. **[REAL, RETRO]** Plastic color should be chosen based on various photos and videos to minimize influence of different weather or white balance on provided footages.
    
11. Downhill lights
    1. Downhill lights are optional. In case of not including lights into hill, "Competition timing" rules apply.
    2. Downhill lights must be not too bright or too dark.
    3. Downhill lights must be not too large or too small.
    4. Illumination of ski jumper during takeoff and flight must be even and bright.
    5. Downhill lights should not use highly saturated colors for main lighting. Color temperatures between 2500K and 5000K are recommended.
    6. Downhill lights may be used for illumination of inrun.
    7. Downhill lights must be attached to the ground or other construction elements.
    8. Downhill ligths must not block ski jumper view during jump.
    9. **[REAL, RETRO]** Downhill lights should be placed and sized in the same way as they are real-life. They may be placed in a different way if their poles will block ski jumper view during jump or will be distractive to players.
    
12. Windflags
    1. Windflags are optional elements of hill. They may be hidden by author.
    2. Windflags should be placed close to downhill fence.
    3. Windflags should be distributed evenly with a reasonable spacing.
    4. Windflags must not block ski jumper view during jump nor be distractive to players.
    
13. Takeoff banner
    1. Takeoff banner is an optional element of hill. It may be hidden by author.
    2. Visible inrun frame should be attached to the front side of takeoff board.
    3. Inrun frame must not block ski jumper view during jump.
    4. **[REAL, RETRO]** Takeoff banner should be used as a replacement for real-life banner, especially when it contains advertisments or logos.


## III. Profile

1. Common rules
    1. Downhill profile must follow a common downhill curve. It must contain only one knoll, one landing zone and one outrun which may be sloped.
    2. K point of hill must be lower or equal than its HS. Hills that do not have HS or its value is unknown, must have HS set to same value as K point.
    3. K point of hill must be greater than its automatically generated P point.
    4. Hill Size must be set to value between 20 and 350 meters.
    5. Hill Size should be set to value between 40 and 300 meters.
    6. Start gates must be distributed in a way that will allow for longer jumps with front winds than with tail wind in ascending order.
    7. Start gates distribution must allow for reasonably safe landing in best conditions (avoid original Bad Mitterndorf HS200).
    8. Downhill profile must not allow for excessive wobbling and losing control in flight due to too high air pressure mid-flight.
    9. Hill profile and start gates distribution should allow to reach K point with any gate available in World Cup mode. This does not apply to RETRO hills without HS value.
    10. Inrun and downhill must be wide enough to prevent from crashing into side border of the hill during a regular jump.
    11. Downhill outrun must be long enough to prevent ski jumper from crashing end of the outrun in World Cup mode.
    
2. **[REAL, RETRO]** Reproducing real profiles
    1. Hills with homologation available should have exactly same parameters as in the document unless there is an other source that suggests a better approach in converting the profile to DSJ4.
    2. In case of no homologation available, hill profile must be recreated as precise as possible using other available sources.
    3. Expected World Record distance in DSJ4 should correlate to real hill record or longest jump performed during official competitions.
    
3. **[FICTIONAL]** Designing fictional profiles
    1. Downhill profile should not allow for too high flight trajectory which could be considered as dangerous in real life.
    2. Downhill and inrun curves must be smooth enough to not allow any excessive bounces or falls.
    3. Hill profile should be substantially different from already verified hills and should not be a copy of a real hill profile.
    4. Hill profile must allow average players to regularly score points. There should be no situation that majority of players score zero points during the competition.
    
4. Inrun guardrail
    1. Inrun guardrail must be set to ensure that ski jumper will not clip through elements of the inrun.
    2. Inrun guardrail must be wide enough to prevent ski jumper being squeezed while going down the inrun.
    3. Inrun guardrail must be narrower than downhill at zero distance.
    
5. Inrun extension
    1. Inrun extension may be used only if there are takeoff board elements that appear after actual takeoff.
    2. Inrun extension, if used, must fit with actual construction/profile elements.
    3. Inrun extension must be used very carefully. It must not cause any issues while doing correct takeoffs, such as instant fall or bouncing off invisible wall.


## IV. Terrain

1. Terrain profile
    1. Terrain profile must be not too sharp or too steep.
    2. Terrain profile must not influence behavior of cameras that follow ski jumper.
    3. Terrain profile must not block ski jumper view during jump.
    4. Inrun and downhill must not be placed under ground level.
    5. **[REAL, RETRO]** Terrain profile should resemble topography relief of the real-life hill. Due to limitations of terrain generation engine, it does not have to look exactly as the real-life one.
    6. **[FICTIONAL]** Terrain profile should reflect topography relief of place where the hill is located. For example, hill located in London should not be surrounded by large mountains.
    7. **[REAL, RETRO]** If downhill of real-life hill is elevated over ground, it must be elevated in game using profile dhill-terrain.
    8. Adjustments of dhill-terrain and inrun-terrain should be used only for elevation adjustment to inrun tower and downhill.
    9. Elevated downhill should not flicker with terrain.
    10. If there is no downhill elevation over ground level visible, profile dhill-terrain should not be defined, unless there is justified need for removal of downhill measurers.
    
2. Trees
    1. Trees must not block ski jumper view during jump.
    2. Trees should be not too small (less than 5-10m) or too large (more than 20-25m).
    3. Trees must not overlap with other hill elements, such as inrun tower, judgetower and other buildings.
    4. Number of trees must not exceed maximum number of trees that current version of game can display (available in Game Settings).
    5. **[REAL, RETRO]** Trees placement should resemble surroundings of the real hill. Due to limitations of trees placement engine, it does not have to look exactly as the real one.
    
3. Blocks and houses
    1. Blocks and houses must not block ski jumper view during jump.
    2. Blocks and houses should not be placed too close to inrun and downhill.
    3. Blocks and houses should not be too large (more than 10-20 floors).
    4. Blocks and houses must not overlap with other hill elements, such as inrun tower, judgetower and other buildings.
    5. Number of blocks and houses must not exceed maximum number of blocks and houses that current version of game can display (available in Game Settings).
    6. **[REAL, RETRO]** Blocks and houses placement should resemble surroundings of the real hill. Due to limitations of blocks and houses placement possibilities, they do not have to be placed in a exactly same way as on the real hill.
    
4. Audience
    1. Number of spectators must not exceed maximum number of spectators that current version of game can display.
    2. Spectators should be placed around outrun of the hill.
    3. Spectators should not be distributed too densely or too sparsely.


## V. Construction elements

1. General
    1. Hill must not include any copyrighted graphics or logos, including those non trademarked. The only exception are graphics for which hill author has explicit permission from their creator.
    2. Hill construction elements should be implemented in a way that will allow small adjustments of profile without having to put too much effort to fix them.
    
2. Optimization
    1. Number of rendered vertices generated in DSJ4 should not exceed 300000. Limit may be increased for hills that contain complex structures or high level of detail.
    2. Hill file should be optimized as much as possible, keeping XML source file readable by humans.
    3. Hill file size should not exceed 512kB. Limit may be increased for hills that contain complex structures or high level of detail.
    4. Number of edges defined in Beams and beamgroups should be as low as possible. For narrow poles or fences, maximum of 8 should be used. To imitate a circular shape, use attribute smooth="true".
    5. Faces that are meant to be invisible or covered by other construction elements should be turned off if possible.
    
3. Ski jumper visibility
    1. Construction elements must not block ski jumper view during performing a jump.
    2. Construction elements must not distract player during performing a jump.
    3. Upper part of inrun (before halfway of transition curve) may be covered by elements that block ski jumper view.
    4. **[FICTIONAL]** Elements placed on upper part of inrun that block ski jumper view should be avoided.
    5. Inrun tracks and their close surroundings must be not covered by any elements that would be distractive or block ski jumper view during performing a jump.
    6. Downhill must be not covered by any construction elements, the only exception are fence elements located on downhill sides.
    
4. 3D models
    1. 3D models should be used only for elements that could be very difficult or impossible to implement with other elements available.
    2. Hill author who designed hill elements in a external 3D editor should save object in its native format to make future object modifications possible.
    3. 3D model should be optimized as much as possible to avoid high vertices count and high file size.
    4. 3D model should use instantiating with object transforms (move, rotate, scale) as often as possible to avoid high file size.
    5. 3D model should not contain any artifacts or incorrectly soft/sharp edges visible.
    
5. Flickering
    1. There must not be any flickering surfaces that are visible from close camera view. Elements that are meant to be not visible or covered by other construction elements are not subject of this rule.
    2. Flickering surfaces and edges caused by high camera distance should be avoided as much as possible.
    
6. Textures
    1. Textures and colors used in hill must be picked to look properly without any Texture Mods.
    2. Pattern of texture applied to long elements should be positioned along the element. This applies especially to wooden railings or fences positioned along inrun or downhill profile.
    
7. **[REAL, RETRO]** Recreating real hill construction elements
    1. Hill construction elements must be designed to resemble look of the recreated hill.
    2. Hill must be recreated based on actual footages of the hill, as recent as possible.
    3. Hill elements that are not visible on any available footage should be designed as simple as possible, following textures and patterns already used in other hill elements.
    4. Proportions of elements should be as close as in the recreated hill.
    5. Some hill elements may be omitted due to their complexity, low significance, being distractive to players, blocking ski jumper view, or not being an integral part of the construction.
    
8. **[FICTIONAL]** Designing fictional hill elements
    1. Hill elements should be realistic and resemble real-life structures.
    2. Inrun tower should contain a visible entrance available from ground level.
    3. Stairs and walkaways placed over ground level, should be covered with proper railings.
    4. Appearance of hill should be significantly different from other hills and should not be a copy of a real hill. Hills that are part of fictional complex may be similar to each other.


## VI. Downhill elements

1. General
    1. Custom downhill elements are optional elements of the hill.
    2. Downhill elements must not be distractive to players.
    3. Hill must have K Point, Hill Size and fall line marked by clearly visible lines.
    4. Fall line must be placed on calculated distance. Attribute refd="f" should be used to define fall line.
    5. Grass may be used only on downhill sides to imitate plastic zone being narrower than downhill.
    6. Number of downhill label instances used should not exceed 15.
    7. Number of custom banner and grass instances combined should not exceed 20.
    8. Number of custom lines instances (summer and winter combined) should not exceed 200. Limit may be increased for very large hills or simple graphics made of custom markings.
    
2. **[REAL, RETRO]** Reproducing real downhill elements
    1. Custom lines, if used, should be placed on exactly same distances as on the real-life hill.
    2. Winter markings layout should be based on layout that was used in recent main events.
    3. Summer markings layout should be based on layout that is currently being in use, or was the latest layout ever used.
    4. Markings layout of hills that do not have plastic downhill in real life, should have layout as simple as possible. Using default markings or same layout as in winter are recommended options.
    5. In case if during recent main event lines were barely visible, completely invisible, earlier or default layout should be used.
    6. Hills that do not have plastic downhill in real life must not be covered entirely with grass or other material.
    
3. Custom text and images on downhill
    1. Placing text or images made of markings (lines, twigs, spray) is allowed.
    2. Text or images made of markings must be simplified as much as possible.
