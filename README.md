# Welcome to Room Designer!

Room Designer is a 2D side-view visualization tool for the early stages of planning a stationary PA system. It helps you configure speaker placement and orientation, estimate SPL (Sound Pressure Level) differentials from the front to the back of an audience, and visualize acoustic coverage on stage. Below is a guide on how to use the tool along with explanations for each control.

---

## Default Setup

**Default Setup:**  
By default, Room Designer is configured for a "run and gun" setup using a JBL SRX815 speaker mounted upright on speaker stands. This provides a baseline scenario that you can modify according to your specific needs.

---

## Getting Started

### 1. Room & Stage Setup
- **Room Dimensions:** Input the overall size of the room. 
- **Audience Position:** Choose whether the audience is seated or standing to adjust acoustic considerations.
- **Stage Height & Length:** Enter the height and length of the stage to accurately represent your performance area.
- **Front Row Distance:** Set the distance from the stage to the front row of the audience. This defines the starting point for coverage calculations.

### 2. Speaker Placement & Orientation
- **Speaker Location:**
  - **Trim Height (Vertical):** Adjust the vertical position of the speaker relative to the stage.
  - **Speaker Position (Horizontal):** Set how far along the stage the speaker is placed.
- **Speaker Angle (Downtilt):** Enter a negative value (e.g., -1°) to tilt the speaker downward. Tilting at least one degree will project an on-axis line, crucial for estimating coverage.
- **Speaker Specifications:** For best results, input all known specifications:
  - Sensitivity
  - Wattage provided
  - Vertical dispersion
  - Horizontal dispersion

### 3. Advanced Features
- **Show Lateral Coverage:** Check this option to calculate Bob McCarthy's Lateral Aspect Ratio multiplier:
  - If the speaker is **upright**, it uses the vertical dispersion spec.
  - If the speaker is **side down**, it uses the horizontal dispersion spec.
  - This helps estimate the length of the speaker’s coverage area over the audience, considering off-axis and distance loss.

### 4. Multiple Speakers
- **Number of Speakers:** Input how many speakers you're using.
- **Phase Selection:**
  - **In Phase:** Doubling speakers increases SPL by 6dB.
  - **Random Phase:** Doubling speakers increases SPL by 3dB.
- **Important:** The multiple speaker feature is for rough estimates only and should not be used for detailed line array calculations.

### 5. Simulation & Estimation
- The tool applies the inverse square law to calculate SPL loss at the intersection of the audience and the speaker’s on-axis line.
- **Important:** Ensure you set a minimum 1° tilt. A speaker aimed completely over the audience will prevent the calculator from working.

### 6. Using the Range Ratio Statistic
- **Aim the Speaker:** Start by angling the speaker to cover the furthest point in the audience.
- **Range Ratio:** This statistic is the ratio of the furthest on-axis throw to the distance to the front row. It estimates the SPL differential between the front and back rows.
  - **Note:** If the range ratio exceeds 4, consider exploring line array, constant curvature, or delay line solutions, as a single point source speaker may not provide adequate coverage.

### 7. Orientation & Units
- Switch between feet and meters depending on your preference.
- Choose whether the stage appears on the right or left side of the view.

---

## Future Enhancements

- **Subwoofer Integration:** There are plans to add subwoofer calculations, which will allow for more comprehensive low-frequency system design.
- **Delay Calculations:** Future updates aim to incorporate delay calculations for better timing and phase alignment in more complex speaker setups.

---

## Important Caveats

- **Early Stage Tool:** Room Designer provides **rough predictions** for the initial stages of a PA system design. It is best used for conceptual planning and should not be relied upon for mission-critical decisions.
- **Not for Detailed Line Arrays:** The multiple speaker feature is not intended for precise line array design calculations. A dedicated line array visualizer tool is in development and will be available in the future.
- **Fan Art Disclaimer:** Room Designer is not endorsed or affiliated with Bob McCarthy. It is a fan-made tool that uses some of his concepts for estimation purposes.

---

## Try it Out

Explore the tool with its default "run and gun" setup using the JBL SRX815, and experiment with different configurations to get a rough idea of how your PA system will perform.  
👉 [Access Room Designer Here](https://nico-avtools.github.io/RoomDesigner/)

Use Room Designer as a creative guide for your initial planning, but always consult with professionals and use more detailed tools as you refine your system design.
