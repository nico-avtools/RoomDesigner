# RoomDesignerRepo
Welcome to RoomDesigner!
RoomDesigner is a 2D side-view visualization tool for the early stages of planning a stationary PA system. It helps you configure speaker placement and orientation, estimate SPL differentials from the front to the back of an audience, and visualize acoustic coverage. 

Getting Started
Defaults Setup: By default, Room Designer is configured for a 40 ft deep by 20ft high room with an audience five rows deep. The speaker spec defaults approximate a typical "run and gun" setup using a JBL SRX815 speaker mounted upright on speaker stands with a ten degree downtilt. This provides a baseline scenario that you can modify according to your needs and rig.
	1.	Room & Stage Setup
	◦	Room Dimensions: Input the overall size of the room.
	◦	Audience Position: Choose whether the audience is seated or standing to adjust acoustic considerations.
	◦	Stage Height & Length: Enter the height and length of the stage to accurately represent your performance area.
	◦	Front Row Distance: Set the distance from the stage to the front row of the audience. This defines the starting point for coverage calculations.
	2.	Speaker Placement & Orientation
	◦	Speaker Location:
	▪	Trim Height (Vertical): Adjust the vertical position of the speaker relative to the stage.
	▪	Speaker Position (Horizontal): Set how far along the stage the speaker is placed.
	◦	Speaker Angle (Downtilt): Enter a negative value (e.g., -1°) to tilt the speaker downward. Tilting at least one degree will project an on-axis line, crucial for estimating coverage.
	◦	Speaker Specifications: For best results, input all known specifications:
	▪	Sensitivity
	▪	Wattage provided
	▪	Vertical dispersion
	▪	Horizontal dispersion
	3.	Coverage Features
	◦	Show Lateral Coverage: Check this option to calculate Bob McCarthy's Lateral Aspect Ratio multiplier:
	▪	This is one method of estimating speaker coverage, projecting the speaker's expanding coverage area onto a 2D surface
	▪	LAR calculation is a multiplier, so it works in both feet and meters
	▪	If the speaker is upright, lateral coverage uses the vertical dispersion spec.
	▪	If the speaker is side down, lateral coverage uses the horizontal dispersion spec. 
	▪	This helps estimate the length of the speaker’s coverage area over the audience (from front to back), estimating combined off-axis and distance loss.
	4.	Multiple Speakers
	◦	Number of Speakers: Input how many speakers you're using.
	◦	Phase Selection:
	▪	In Phase: Doubling speakers increases SPL by 6dB.
	▪	Random Phase: Doubling speakers increases SPL by 3dB.
	◦	Important: The multiple speaker feature is for rough estimates only and should not be used for line array calculations, which have more complex interactions.
	5.	SPL Estimation
	◦	The tool applies the inverse square law to calculate SPL loss at the intersection of the audience and the speaker’s on-axis line.
	◦	Important: Ensure you set a minimum 1° tilt. A speaker aimed completely over the audience will prevent the calculator from working.
	6.	Using the Range Ratio Statistic
	◦	Aim the Speaker: Start by angling the speaker to cover the furthest point in the audience.
	◦	Range Ratio: This statistic is the ratio of the furthest on-axis throw to the distance to the front row. It estimates the SPL differential between the front and back rows.
	▪	Note: If the range ratio exceeds 4, consider exploring line array, constant curvature, or delay line solutions, as a single point source speaker may not provide adequate coverage.
	7.	Orientation & Units
	◦	Switch between feet and meters depending on your preference.
	◦	Choose whether the stage appears on the right or left side of the view.

Important Caveats
	•	Early Stage Tool: Room Designer provides rough predictions for the initial stages of a PA system design. It is best used for conceptual planning and should not be relied upon for mission-critical decisions.
	•	Not for Line/Constant Curvature Arrays: The multiple speaker feature is not intended for precise line array design calculations. I am working on a line array calculator tool.
	•	Mains Only: This tool does not have any functionality for incorporating subs or delay speakers. I hope to add these features.
	•	Disclaimer: Room Designer is not endorsed by or affiliated with Bob McCarthy. It is a fan-made tool that uses some of his concepts for estimation purposes. Any errors are my own. 
