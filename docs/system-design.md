# Functional structure and workflow

I created the functional structure block diagram and wrote the full operating-workflow explanation. The diagram defines the machine boundary and the exchanges of eggs, oil, eggshell waste, electrical energy, control signals, and feedback.

[Open the complete report section 4 (4.1-4.6)](system-design/SunnyPro_Functional_Structure_and_Workflow.pdf) - full-report pages 54-66.

## Scope

The workflow describes preparation, startup, temperature settings, preheating, user input, egg release and detection, cracking, shell collection, conveyor loading, oil dosing, heating, monitoring, serving, refilling, waste removal, and shutdown.

The subsystem descriptions connect a physical task to the relevant actuator or sensor. This helped organise the interfaces between the conveyor, heating systems, serving platform, display, and the egg-handling mechanisms.

## Sequence and implementation status

Oil dosing is intended to prepare the cooking pocket before egg deposition, as described in the oil pre-spray calculation. The workflow narrative and detailed process timing need a final consistency review before a controller is implemented.

The functional block diagram describes system relationships. It is distinct from the team's detailed program flowcharts, which remain available in the full report; authorship of those flowcharts is not claimed here.

No firmware implementation, automatic operation, fault-response test, or physical interlock test is demonstrated by these documents.
