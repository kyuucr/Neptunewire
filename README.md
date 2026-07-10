# Elegoo Neptune 3 to Switchwire Conversion 

This is a full conversion of the Elegoo Neptune 3 to a Voron Switchwire, originally forked from [boubounokefalos](https://github.com/boubounokefalos/Ender_SW)'s Ender 3 conversion with prior work by [Triano](https://github.com/walttriano/VoronUsers/tree/master/printer_mods/Triano/Ender_3Pro_Switchwire). Electronics mounting based on Fizzy's Tech's [EMS](https://www.printables.com/model/477791-ft-ems-v02-electronic-management-system)

This is an ongoing work that attempts to continue [robertsamples](https://github.com/robertsamples/Neptunewire)'s work. I can confirm at this point that I successfully printed and installed the parts as well as confirmed that the core XZ kinematic is working. Do not expect BOM very soon but you can start from [the original BOM](https://github.com/walttriano/VoronUsers/raw/refs/heads/master/printer_mods/Triano/Ender_3Pro_Switchwire/BOM/SW_to_E3P_BOM.xlsx) with the additions of longer M3, M4, and M5 SHCS. Plan to buy an assortment of 30-50 mm in 5mm increments for each of these. Longer M5s are essential for the top Z bar with the sandwiched idlers. Some not-voron standard heatset inserts are required in M5 size (I used L=5.8mm, top OD=7.1mm, bottom OD=6.3mm).

## Todo

- [ ] Share an example printer.cfg.

- [ ] Create a 4040 MGN12 guide for the Y linear rails that can be used without removing deck panels.

- [ ] Update CAD with Dragon Burner v8 models.

## Changelogs

### v0.1

- Fixed folder and file names to align more to Voron community's naming convention.

- Finished modification of deck panels, splitting the left and right decks into two parts (front and back) instead of Enderwire's three parts. Confirmed to be printable on Neptune 3's 235x235 mm print area.

- Added rear middle grill.

- Added mirrored 4040 deck mount STLS that anchors the deck panels, with the right side also anchors the Z cable chain.

- Added power supply mount and blank hex electronics mount STLs, as well as a mount with mounting points for BTT SKR Pico and Mellow FLY-UTOR I personally used.

- Added back lcd_blank.stl from the original Switchwire and removed STLs related to Ender's screen since Neptune 3's screen is proprietary and seems difficult to reuse. I personally plan to use BTT HDMI5 and there are already Switchwire mounting mods that can be reused for this conversion.

- Added back Y Motor Mount Bracket from Enderwire, there are some attempts to modify the bracket but I am unsure about the original intention.

- Added nut holes to rear extensions instead of heatsets with plugs to hold the nuts in place.

- Added back XZ Gantry STLs from Switchwire that are required for the conversion.

### v0 (original robertsamples)

- Modified the xz idlers on top beam to sandwich between the extrusions so drilling a new extrusion is not required.

- Bottom cross member moved forward instead of just the y extrusion due to the Neptune 3's differences in mounting holes, adding 90 degree brackets is a good idea for rigidity.

- The motor extender on the y axis is required and extra heatset insert points have been added to compensate for the lack of mounting options on the N3s closed extrusions.

- Electronics and PSU are mounted in the front with a printable bracket to secure the PSU and electronics (NOT UPDATED IN CAD YET).

- Electronics mounting points are for the Mellow Gemini V3, but the hex mounts can be easily modified for whatever klipper host and main board you have.

- Key back mount modified to work with the for the N3s PSU mount holes.

- A regular 2020 extrusion for the gantry needs to be added.
  
- option for XZ idlers on gantry added that use short M5 heatset inserts.
  
- Deck Panels modified for Neptune 3, I have access to a larger printer so you may need to modify the CAD accordingly. Only left side fully modified but this can be used as a template. Bottom deck modified to add holes for ventilation of the N3 PSU.
  
- Enclosure panels extended to accomodate the height of the N3.
  
- Experimental dragonburner carriage added (extra mounting points for V6 dragonburner with modified cowl only currently, V7 can be used but will not have heatsets for additional rigidity).

- Mirrored cable chain deck mount and added anchor to side of N3 extrusions.
  
- Extra holes for heatsets added on the Y extenders and bottom bar that the feet mount to to allow for screws to further secure the bottom bar to the frame since they can't be secured to the closed extrusions on the bottom as usual with t slot nuts (NOT UPDATED IN CAD YET).
