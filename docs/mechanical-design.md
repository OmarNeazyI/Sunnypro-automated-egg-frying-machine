# Mechanical design, component selection, and functional calculations

I selected components and performed the functional calculations for the subsystems I developed. The source calculations are preserved separately:

- [Selected functional calculations](calculations/SunnyPro_Functional_Calculations.pdf): report pages 67-75, 82-86, and 111-125.
- [Purchased-component requirements](components/SunnyPro_Purchased_Component_Requirements.pdf): report pages 207-226.
- [Final BOM](bom/SunnyPro_Final_BOM.pdf): report pages 241-254.

The calculations PDF retains contextual team work alongside the conveyor, rotating-platform, oil-dosing, and cooking calculations. Inclusion of a source page does not assign all of its authorship to me.

## Conveyor and drive

The design uses two parallel 06B-1-K1 chains and four cooking plates. My CAD work includes the shafts, sprockets, supports, conveyor structure, plate arrangement, and drive integration.

The drive-sizing section uses a NEMA 17 stepper, a 27:1 gearbox arrangement, and a TB6600 driver. It calculates a translating load of approximately 3.27 kg, including assumptions for eggs and minor items. This is a design estimate using CAD and catalogue inputs, not a weighed assembly.

The calculation relates linear travel to sprocket speed, gearbox speed, acceleration, torque, and step resolution. Step resolution is a commanded increment and does not establish actual positioning accuracy.

[Conveyor and drive - original CAD screenshot](../assets/images/conveyor-and-drive.png)

## Rotating serving platform

My assembly includes the plate, bearing support, load-cell support parts, base platform, motor casing, friction-drive arrangement, and microswitch reference features.

The documented concept uses a 28BYJ-48 geared stepper and a friction wheel against the plate rim. The drive calculation describes 90-degree indexing, the wheel-to-plate ratio, rotational loading, and a microswitch home reference. Friction slip, backlash, switch repeatability, and available running torque were not physically tested.

[Platform view](../assets/images/rotating-platform.png) | [Side view](../assets/images/rotating-platform-side.png)

## Heating assemblies

The top assembly combines my custom shield, supports, protective perforated sheet, and mounting features with a simplified representation of the purchased quartz heating element.

The lower assembly includes the aluminium heating block, heater and sensor locations, surrounding frame, and mounting brackets.

I selected the relevant components and performed the subsystem's functional calculations, with a supporting contribution to the heating calculations. The report's cooking model is an analytical/numerical design estimate; its implementation and predictions have not been independently reproduced or experimentally validated in this project.

[Top shield](../assets/images/top-ir-shield.png) | [Shield end view](../assets/images/top-ir-shield-end.png) | [Bottom heating assembly](../assets/images/bottom-heating-assembly.png)

## Eggshell drawer

I designed the rail-supported drawer and the compression mechanism. The model includes the intended sliding and pressing movement.

[Rails retracted](../assets/images/eggshell-drawer-closed.png) | [Rails extended](../assets/images/eggshell-drawer-open.png)

Drawer capacity, required compression force, sealing, wear, and cleaning performance remain untested. The CAD positions alone do not validate those characteristics.

## Oil storage

I designed the oil tank and its mounting arrangement, selected the subsystem components, and performed the relevant functional calculations. The report documents a proposed peristaltic pump, tubing, check valve, and nozzle arrangement. Their combined dose, spray coverage, and compatibility with the selected oil remain untested.

## Display assembly

I designed the display casing, including the front and rear parts, fixing features, and mounting assembly. The screen module itself is a purchased component.

[Display casing](../assets/images/display-casing.png) | [Rear casing and mounting assembly](../assets/images/display-mount-rear.png)

## Calculations and open consistency checks

The cooking calculation uses approximately 19.3 mm/s over a 450 mm heating zone, whereas the conveyor drive-sizing section uses 30 mm/s over a 666.51 mm straight. These are different design cases, not a single demonstrated operating point. A final baseline must reconcile heating length, dwell/index behaviour, plate spacing, and motor commands.

The rotating-platform timing also needs reconciliation with the selected conveyor cycle. A motor's holding-torque specification does not by itself establish available running torque or prove that missed steps cannot occur.

See [design status](design-status.md) for the remaining limitations.
