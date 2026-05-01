# SKILL LAB PRATICAL HACKATHON

## Final Project README

> **Project Weight:** 100%  
> **Team Size:** 4/3 students  
> **Project Duration:** 16 hours  
> **Total Time Available:** 32 effort-hours per team  
> **Project Type:** Playful, interactive, technology-based experience

---

# Before you begin

## Fork and rename this repository

After forking this repository, rename it using the format:

`SKILLLAB_PROR-2026-TeamName`

### Example

`SKILLLAB_PROR-2026-AuroWizards`

Do not keep the default repository name.

---

# How to use this README

This file is your team’s **working project document**.

You must keep updating it throughout the build period.  
By the final review, this README should clearly show:

- your idea,
- your planning,
- your design decisions,
- your technical process,
- your build progress,
- your testing,
- your failures and changes,
- your final outcome.

## Rules

- Fill every section.
- Do not delete headings.
- If something does not apply, write `Not applicable` and explain why.
- Add images, screenshots, sketches, links, and videos wherever useful.
- Update task status and weekly logs regularly.
- Use this file as evidence of process, not only as a final report.

---

# 1. Team Identity

## 1.1 Studio / Group Name

`Project^2`

## 1.2 Team Members

| Name                  | Primary Role                    | Secondary Role   | Strengths Brought to the Project |
| --------------        | ------------------------------- | --------------   | -------------------------------- |
| `Neev Jain `          | `Software(Flask/App)`           | `UI Design`      |  `Coding ,Logic Building `       |
| `Hitesh Gughe`        | `Hardware (sensors)`            | `Circuit Setup`  | `Electronics , Wiring`           |
| `Bharati Bhatia`      | `Software(Backend/UI)`          | `Testing`        | ` Problem Solving , UI`          |
| `Sanika Shahasane`    | `Hardware (Integration)`        | `Documentation`  | `Hardware Integration`           |

## 1.3 Project Title

`Smart Parking System using Raspberry Pi and IR Sensors`

## 1.4 One-Line Pitch

`A smart parking system that detects slot availability using sensors and allows users to book parking slots through a web interface.`

## 1.5 Expanded Project Idea

In 1–2 paragraphs, explain:

- what your project is,
- what kind of experience it creates,
- what technologies are involved.

**Response:**  
`Our project is a Smart Parking System that combines both hardware and software. IR sensors are used to detect whether a parking slot is occupied or free. These sensors are connected to a Raspberry Pi, which reads the sensor data using GPIO pins.The Raspberry Pi sends this data to a Flask-based web application. Users can log in, view available slots, and book parking. The system updates slot availability dynamically based on sensor input.
This integration of hardware and software makes the system practical and suitable for real-world parking management.`

---

# 2. Inspiration

## 2.1 References

List what inspired the project.

| Source Type | Title / Link                            | What Inspired You                                       |                                                | Web         | Smart Parking System (YouTube / Google) | Concept of using sensors to detect parking availability |
| Website     | https://www.raspberrypi.com             | Use of Raspberry Pi for hardware control                |
| Concept     | IoT Parking Systems                     | Integration of sensors with web application             |

## 2.2 Original Twist

What makes your project original?

**Response:**  
`Our project is not just a basic parking system. We combined hardware (IR sensors and Raspberry Pi) with a web-based booking system.
The originality lies in integrating real-time sensor data with a user-friendly web interface. Users can not only view slot availability but also book parking slots online, see pricing, and manage bookings.This makes the system more practical and interactive compared to traditional parking systems which only display availability`

---

# 3. Project Intent

## 3.1 User Journey 

Describe exactly how a user will use the project.Make it a story
**Response:**  
`A user first signs up and logs into the system through the web application. After logging in, the user sees the dashboard displaying available parking slots.
The slot availability is updated based on IR sensor readings connected to the Raspberry Pi. If a vehicle is present, the sensor detects it and marks the slot as occupied.The user selects a vehicle type, enters vehicle details, and books a parking slot. The system calculates the cost and confirms the booking.
If all slots are occupied, the system displays "Parking Full" and disables booking.`
                                                  |

---

# 4. Definition of Success

## 4.1 Definition of “Usable”
`A system is considered usable when both hardware and software components work correctly together.The user should be able to easily sign up, log in, view available slots, and book a parking slot without confusion. At the same time, the IR sensors should correctly detect whether a slot is occupied or free, and the Raspberry Pi should update the system accordingly.The interface should be simple, and the system should respond accurately in real-time.`


## 4.2 Minimum Usable Version

What is the smallest version of this project that still delivers the core experience?

**Response:**  
`The minimum usable version includes a working web application where users can log in and book parking slots, along with at least one IR sensor connected to the Raspberry Pi.The sensor should detect slot occupancy and update the system accordingly. Even with one sensor, the system should demonstrate real-time detection and booking functionality.`

## 4.3 Stretch Features

What features are nice to have but not essential?

`- Multiple IR sensors for detecting multiple parking slots
- Real-time slot updates using Raspberry Pi GPIO
- Visual slot representation on dashboard
- Booking history and cancellation feature
- Integration with mobile notifications (future scope) `

---

# 5. System Overview

## 5.1 Project Type

Check all that apply.

- [x] Electronics-based

- [ ] Mechanical

- [x] Sensor-based

- [x] App-connected

- [x] Motorized

- [ ] Sound-based

- [x] Light-based

- [x] Screen/UI-based

- [x] Fabricated structure

- [x] Game logic based

- [x] Installation

- [ ] Other:

## 5.2 High-Level System Description

Explain how the system works in simple terms.

Include:

- input,
- processing,
- output,
- physical structure,
- app interaction if any.

**Response:**
`The system consists of both hardware and software components.
Input:
IR sensors are used as input devices. They detect whether a parking slot is occupied or free based on object detection.
Processing:
The IR sensors are connected to a Raspberry Pi. The Raspberry Pi reads sensor data through GPIO pins and processes whether the slot is available or not.
Output:
The processed data is sent to a Flask-based web application. The website displays available slots, booking status, and pricing.
Physical Structure:
Each parking slot has an IR sensor installed. All sensors are connected to the Raspberry Pi, which acts as the central controller.
App Interaction:
Users interact with the system through a web interface. They can log in, check availability, and book parking slots. The system updates slot availability dynamically. `

## 5.3 Input / Output Map

| System Part      | Type       | What It Does                                  |
| IR Sensor        | Input      | Detects vehicle presence                      |
| Raspberry Pi     | Processing | Reads sensor data and processes slot status   |
| GPIO Pins        | Interface  | Connect sensors to Raspberry Pi               |
| Flask App        | Processing | Handles user interaction and booking          |
| SQLite Database  | Storage    | Stores user and booking data                  |
| Web Dashboard    | Output     | Displays available slots and booking info     |

---

# 6. System Design, Sketches and Visual Planning 

## 6.1 Concept Architecture/sketch/schematic

Add an early sketch of the full idea.

**Insert image below:**  
`[
]`


Example:

```md

```



## 6.2 Labeled Build Sketch/architecture/flow diagram/algorithm

Add a sketch with labels showing:

- structure,
- electronics placement,
- user touch points,
- moving parts,
- output elements.

**Insert image below:**  
`[Upload image and link here]`
>
<img width="1080" height="1534" alt="WhatsApp Image 2026-05-01 at 7 48 17 PM" src="https://github.com/user-attachments/assets/fee6628e-0725-4f7d-9d2f-de17703ec155" />

## 6.3 Approximate Dimensions

| Dimension        | Value   |
| ---------------- | ------- |
| Length           | `16 cm` |
| Width            | `16 cm` |
| Height           | `8 cm`  |
| Estimated weight | `400 g` |

---

# 7. Electronics Planning

## 7.1 Electronics Used

| Component                 | Quantity | Purpose                               |
| ------------------------- | --------:| ------------------------------------- |
| `[Raspberry Pi]`          | `1`      | `[Main controller]`                   |
| `[IR Sensors]`            | `2`      | `[Vehicle detection]`                 |
| `[PyCam/Webcam]`          |  `1`      | `[To detect type of vehicle]`        |
| `[LEDs]`                  | `1`      | `[To confirm a vehicle]`              |
| `[I2C LCD]`               |` 1` |`[Displays booking status]`  |
|` [Touch Sensors]` |` 1` | ` [To control the barricade]` |
|`[Buzzer]`|`1`|`[for illegal entry]`|
|`[LEDs]`|`[2]`|`[Slot booking]`|
## 7.2 Wiring Plan

Describe the main electrical connections.

**sample Response:**  
`The RASPI is connected to the I2C LCD using four GPIO pins (2,6,3,5) to I2C pins (5V, GND, SDA, SCL) respectively.
 
 The two IR sensors using three GPIO pins (1,6,11) and (1,6,12) to 3.3V, GND and output respectively.
 
 The Touch Sensor to GPIO pins (1,6,13).

The two LEDs are connected to GPIO 15 and 16 and a buzzer is connected to GPIO 18.
`

## 7.3 Circuit Diagram/architecture diagram

Insert a hand-drawn or software-made circuit diagram.

**Insert image below:**  
`[(https://drive.google.com/file/d/1LkzW4oW6XcjPHx7QGRLeFAiQvFghBp-7/view?usp=sharing)]`
<img width="867" height="1156" alt="" src="" />
<img width="1600" height="1167" alt="WhatsApp Image 2026-05-01 at 8 25 30 PM" src="https://github.com/user-attachments/assets/f176d6dd-c193-42cf-9aa1-1a3d5627adf6" />


# 7.4. Power Plan

| Question         | Response                                                                                                                                          |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| Power source     | `Power Suppy switch`                                                                                                                           |
| Voltage required | `~5V`                                                                  |
| Current concerns | `Raspi draws 600mA-1.2A`                                       |
| Safety concerns  | `If you smell "hot electronics," unplug the USB power immediately. Usually, that’s a sign of a short circuit or a component drawing too much current.` |

---

# 8. Software Planning/

## 8.1 Software Tools

| Tool / Platform                | Purpose                                        |
| ------------------------------ | ---------------------------------------------- |
| `[Raspberry Pi Terminal]`      | `Control RaspberryPi`                          |
| `[Python/OpenCV]`              | `Vehicle Type Detection` |
| `[Flask]` | `[Backend/API]`                      |


## 8.2 Software Logic/Algorithm

Describe what the code must do.

Include:

- startup behavior,
- input handling,
- sensor reading,
- decision logic,
- output behavior,
- communication logic,
- reset behavior.

**Response:**  
`
**Startup Behavior**

The system initializes in two distinct environments:Hardware (Raspberry Pi): The GPIO pins are configured using the BCM mode. Pins are assigned to specific roles: IR and Touch sensors as inputs, and LEDs (Green/Red) and a Buzzer as outputs. The I2C LCD is initialized to display status messages.  Web Server (Flask): The application sets up API blueprints and dashboard routes. It requires an API key (PI_API_KEY) to be configured for secure communication with the hardware.  

**Input Handling**

The system processes three primary forms of input:Physical Sensors: It monitors an IR sensor (pin 17) for vehicle presence and a Touch sensor (pin 27) for manual assistance requests.  User Interaction: Users interact via a web dashboard to book slots, while admins manage users and export data.  API Payloads: The backend accepts JSON payloads containing slot_code and is_occupied boolean values. 

**Sensor Reading**

The hardware logic continuously polls the digital inputs in a loop:Presence Detection: GPIO.input(IR) returns True if a vehicle is detected in the slot.  Touch Input: GPIO.input(TOUCH) is checked while a vehicle is present to trigger specific "Assist" logic.

**Decision Logic**

The Raspberry Pi script manages state transitions based on sensor timing and input:Idle Logic: If the IR sensor is not triggered, the system remains in a "Slot Available" state.  Detection Timer: Once a vehicle is detected, a timer starts. If the vehicle stays for more than 5 seconds without clearing the sensor, the system decides it is "Wrong Parking" (misaligned).  Assist Logic: If the touch sensor is activated during detection, it overrides other messages to display "Assist Mode".  Occupancy Confirmation: Once the IR sensor is no longer triggered after a detection event, the system concludes the slot is now "Occupied".

**Output Behavior**

The system provides real-time feedback through multiple channels:Visual (Hardware): A Green LED indicates availability or active detection, while a Red LED indicates a "Wrong Parking" error or a finalized "Occupied" status.  Audio: A buzzer sounds during "Assist Mode" or to alert the driver to adjust their vehicle.  LCD Display: Shows text updates such as "Slot Available," "Adjust Vehicle," or "Slot Occupied".  Web UI: The dashboard updates a "Live Parking Status" and can trigger a "Wrong parking detected!" popup for users. 

**Communication Logic**

Communication between the hardware and the server is handled via a REST API:The system uses POST requests to /api/sensor/update.  Security: Requests must include an X-API-KEY in the header to be authorized.  Data Parsing: The server normalizes various input types (e.g., "1", "true", "occupied") into standard boolean values to update the database. 

**Reset Behavior**

The system handles resets and shutdowns through two mechanisms:Cleanup: Upon a KeyboardInterrupt (manual stop), the hardware script executes GPIO.cleanup(), which resets all pins to a safe state to prevent hardware damage or lingering signals.  Looping: The main logic is wrapped in a while True loop, ensuring that after a vehicle occupies a slot or an error is cleared, the system returns to its monitoring state. 

`

## 8.3 Code Flowchart

Insert a flowchart showing your code logic.

Suggested sequence:

- start,
- initialize,
- wait for input,
- read input,
- decision,
- trigger output,
- repeat or reset,
- error handling.

**Insert image below:**  
<img width="1600" height="1200" alt="image" src="" />
<img width="1600" height="1200" alt="image" src="" />




# 9. Bill of Materials

## 9.1 Full BOM

| Item                             | Quantity | In Kit? | Need to Buy? | Estimated Cost | Material / Spec               | Why This Choice?          |
| -------------------------------- | --------:| ------- | ------------ | --------------:| ----------------------------- | ------------------------- |
| `[RASPI]`                        | `1`      | `Yes`   | `No`         | `0`            | `38 Pin ESP32`                | `[To control components]` |
| `[I2C LCD]`                 | `[1]`    | `[Yes]` | `[No]`       | `0`            |                    | `[Displays booking status]`  |
| `[IR Sensors]`          | `[2]`    | `[Yes]`  | `[No]`      | `[0]`        | | `[Vehicle detection]`    |
| `[Touch Sensor]`               | `[1]`    | `[yes]`  | `[No]`      | `[0]`         |                               |     `[Automates barricade operation instead of operating manually`                      |
| `[Buzzer]` | `[1]`    | `[Yes]`  | `[No]`      | `[0]`        |                              |     ` [Intrusion detedtion]`                      |

## 9.2 Material Justification

Explain why you selected your main materials and components.

**Response:**  
`**Main Controller**: 

 Raspberry PiThe Raspberry Pi serves as the central hub because it possesses the GPIO (General Purpose Input/Output) capabilities necessary to interface with       physical sensors while simultaneously running high-level Python logic. It handles the "Main" loop that manages timing for "Wrong Parking" logic and facilitates    the communication logic required to send HTTP POST requests to the Flask web server. 

**Vehicle Detection**: 

 IR SensorsIR (Infrared) Sensors were selected for primary vehicle detection because they provide a simple digital signal (True or False) to indicate presence. In  the code, the IR sensor (Pin 17) acts as the trigger for the entire detection sequence, allowing the system to distinguish between an empty slot and a "Vehicle    Detected" state. 

**User Feedback**: I2C LCD & LEDs
 
 I2C LCD: This component is critical for providing clear, human-readable instructions to the driver, such as "Slot Available," "Adjust Vehicle," or "Slot           Occupied". Using the I2C protocol allows the display to be controlled using only two data pins, saving GPIO space for other sensors.  
 LEDs: The Green and Red LEDs provide instant visual confirmation of the slot's status. Green signals that the slot is ready or a vehicle is being detected, while  Red signals an error (Wrong Parking) or that the booking is finalized and the slot is occupied. 

**Interaction & Security**: Touch Sensor & Buzzer
 
 Touch Sensor: This component acts as a manual override or "Assist Mode" trigger. When a user interacts with it, the system enters a specific logic branch that     activates the buzzer and updates the LCD, providing a physical interface for the driver to request help. 
 Buzzer: The buzzer is used as an audible alert system. It is strategically triggered when the system detects "Wrong Parking" (vehicle misaligned for more than 5   seconds) or when "Assist Mode" is activated, ensuring the driver is alerted even if they are not looking at the LCD or LEDs. 

**Backend Integration**:
 
 Web APIWhile not a physical "material," the Flask API and Dashboard components (referenced in user dashboard html code.txt and api generator code.txt) are         justified by the need for remote monitoring. This allows the "Live Parking Status" to be viewed on a web browser, translating the physical sensor data into        actionable information for both users and administrators.  `


## 9.3 Items You chose

| Item                 | Why Needed               | Purchase Link | Latest Safe Date to Procure | Status       |
| -------------------- | ------------------------ | ------------- | --------------------------- | ------------ |
| `I2C LCD`            | `Display`                |               |                             | `[Received]` |
| `IR Sensors`         | `Sensor devices`         |               |         | `[Received]` |
| `Li-ion Batteries`   | `Portable power`         | `local store` | `before testing`            | `Recieved`   |

## 9.4 Budget Summary

| Budget Item           | Estimated Cost              |
| --------------------- | ---------------------------:|
| Electronics           | `[400]`                     |
| Mechanical parts      | `[200]`                     |
| Fabrication materials | `[0 (Available on campus)]` |
| Purchased extras      | `[0]`                       |
| Contingency           | `[300]`                     |
| **Total**             | `[900]`                     |

## 9.5 Budget Reflection

If your cost is too high, what can be simplified, removed, substituted, or shared?

**Response:**  

---

# 10. Planning the Work

## 10.1 Team Working Agreement

Write how your team will work together.

Include:

- how tasks are divided,
- how decisions are made,
- how progress will be checked,
- what happens if a task is delayed,
- how documentation will be maintained.

**Response:**  


## 10.2 Task Breakdown

| Task ID | Task                    | Owner    | Estimated Hours | Deadline     | Dependency | Status |
| ------- | ----------------------- | -------- | ---------------:| ------------ | ---------- | ------ |
| T1      | `[Finalize concept]`    | `[Both]` | `2`             | `1st April`  | `None`     | `Done` |


## 10.3 Responsibility Split

| Area                 | Main Owner     | Support Owner |
| -------------------- | ----------     | ------------- |
| Concept              | `[Mrugendra]`  | `[Jyoti]`     |
| Electronics          | `[]`           | `[]`          |
| Coding               | `[]`           | `[]`          |
| Mechanical build     | `[]`           | `[]`          |
| Testing              | `[]`           | `[]`          |
| Documentation        | `[]`           | `[]`          |

---

# 11 hour Milestones

## 11.1 8-hour Plan(tentetively you may set)

### Bi Hour 1 — Plan and De-risk

Expected outcomes:

- [x] Idea finalized
- [x] Core interaction decided
- [x] Sketches made
- [x] BOM completed
- [x] Purchase needs identified
- [ ] Key uncertainty identified
- [x] Basic feasibility tested

### Bi Hour 2 — Build Subsystems

Expected outcomes:

- [x] Electronics tests completed
- [ ] CAD / structure planning completed
- [ ] App UI started if needed
- [x] Mechanical concept tested
- [x] Main subsystems partially working

### Bi Hour 3 — Integrate

Expected outcomes:

- [x] Physical body built
- [x] Electronics integrated
- [x] Code connected to hardware
- [ ] App connected if required
- [x] First playable version exists

### Bi Hour 4 — Refine and Finish

Expected outcomes:

- [x] Technical bugs reduced
- [x] Playtesting completed
- [x] Improvements made
- [x] Documentation completed
- [x] Final build ready

## 12.2  Update Log

| Days   | Planned Goal   | What Actually Happened | What Changed   | Next Steps     |
| ------ | -------------- | ---------------------- | -------------- | -------------- |
| Day 1 | `[Write here]` | `[Write here]`         | `[Write here]` | `[Write here]` |
| Day 2 | `[Write here]` | `[Write here]`         | `[Write here]` | `[Write here]` |
| Day 3 | `[Write here]` | `[Write here]`         | `[Write here]` | `[Write here]` |
| Day 4 | `[Write here]` | `[Write here]`         | `[Write here]` | `[Write here]` |

---

# 13. Risks and Unknowns

## 13.1 Risk Register

| Risk                                                            | Type         | Likelihood | Impact   | Mitigation Plan                                                                       | Owner                |
| --------------------------------------------------------------- | ------------ | ---------- | -------- | ------------------------------------------------------------------------------------- | -------------------- |
| WiFi connection between laptop and ESP32 becomes unstable       | `Technical`  | `Medium`   | `High`   | Keep ESP32 close, ensure stable power supply, reduce network load, add fail-safe stop | `[Gopal]`           |


## 13.2 Biggest Unknown Right Now

What is the single biggest uncertainty in your project at this stage?

**Response:**  


---

# 14. Testing 

## 14.1 Technical Testing Plan

| What Needs Testing     | How You Will Test It                                                                 | Success Condition                                                                                    |
| ---------------------- | ------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------- |
| `[Wifi connection]`    | `[Check if motor spins via app button]`                                              | `[Both motors accurately respond to wifi signals]`                                                   |
                       |
## 14.2 Testing and Debugging Log

| Date          | Problem Found                         | Type         | What You Tried                                | Result               | Next Action                                    |
| ------------- | ------------------------------------- | ------------ | --------------------------------------------- | -------------------- | ---------------------------------------------- |
| `18th April`  | `Car not balancing properly`          | `Mechanical` | `Add low-friction caster support to one side` | `Worked`             | `improve caster structure`                     |


## 14.3 Playtesting Notes

| Tester      | What They Did                        | What Confused Them                    | What They Enjoyed                         | What You Will Change                          |
| ----------- | ------------------------------------ | ------------------------------------- | ----------------------------------------- | --------------------------------------------- |
| `Gopal` | `Tried navigating through obstacles` | `Some obstacles ewren't clear enough` | `Liked projection + real car interaction` | `Add a slight red highlight around obstacles` |


---

# 15. Build Documentation

## 15.1 Fabrication Process(if any)

Describe how the project was physically made.

Include:

- cutting,
- 3D printing,
- assembly,
- fastening,
- wiring,
- finishing,
- revisions.

**Response:**  
`The fabrication process involved designing, manufacturing, assembling, and refining both the physical structure and electronic integration of the system.`

`Design (CAD Modeling):
The initial model was created using CAD software, where components were designed based on the actual dimensions of the electronic parts. This ensured accurate fitting and minimized errors during assembly.
Cutting (Laser Cutting):
The designed parts were fabricated using laser cutting techniques. Sheets were cut precisely according to the CAD model to create the structural base and mounts for components.`

`Components were fixed using adhesives and mechanical supports. Certain parts were intentionally kept modular (not permanently fixed) to allow easy replacement and modification of electronics.
Surface Finishing:
Some parts were sanded to smooth rough edges after cutting. Sawdust mixed with adhesive was used to fill gaps and uneven edges, improving structural finish. The final structure was then painted for better aesthetics and durability.`

`Environment Setup (Dark Room Fabrication):
To enhance projection visibility, a controlled dark environment was created using Z-boards, paper sheets, and bedsheets. This minimized external light interference and improved projection clarity.
Revisions and Iterations:
Multiple adjustments were made throughout the process, including refining alignment, improving structural stability, repositioning components, and optimizing the interaction between the physical car and projected environment.`

## 16 Build Photos

Add photos throughout the project.

Suggested images:

- early sketch,
- prototype,
- electronics testing,
- mechanism test,
- app screenshot,
- final build.
- <img width="960" height="1280" alt="WhatsApp Image 2026-04-24 at 9 46 02 AM (1)" src="https://github.com/user-attachments/assets/74baa570-5770-483e-be6d-d2f03386e37c" />





# 17. Final Outcome

## 17.1 Final Description

Describe the final version of your project.

**Response:**  


## 17.2 What Works Well



## 17.3 What Still Needs Improvement


## 17.4 What Changed From the Original Plan

How did the project change from the initial idea?

**Response:**  


---

# 18. Reflection

## 18.1 Team Reflection

What did your team do well?  
What slowed you down?  
How well did you manage time, tasks, and responsibilities?

**Response:**  


## 18.2 Technical Reflection

What did you learn about:

- electronics,
- coding,
- mechanisms,
- fabrication,
- integration?

**Response:**  


## 18.3 Design Reflection

What did you learn about:

- designing ,
- delight,
- clarity,
- physical interaction,
- understanding,
- iteration?

**Response:**  


## 18.4 If You Had One More hour

What would you improve next?

**Response:**  

` `

---

# 19. Final Submission Checklist

Before submission, confirm that:

- [x] Team details are complete
- [x] Project description is complete
- [x] Inspiration sources are included
- [x] Sketches are added
- [x] BOM is complete
- [x] Purchase list is complete
- [x] Budget summary is complete
- [x] Mechanical planning is documented if applicable
- [ ] App planning is documented if applicable
- [x] Code flowchart is added
- [x] Task breakdown is complete
- [x] Weekly logs are updated
- [x] Risk register is complete
- [x] Testing log is updated
- [x] Playtesting notes are included
- [x] Build photos are included
- [x] Final reflection is written
<img width="1131" height="1600" alt="image" src="" />

---


---


