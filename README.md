# SafetyConnect Wristband

## Project Overview:  
is a discreet, wearable, and protective wristband that detects alcohol and gas leaks that alerts the user and their parents and/or guardian. Unlike reactive seafety measures, this wristband autonomously detects environmental hazards specifically **Alcohol (Ethanol)** and **Natural Gas** and bridges the communication gap between a minor and their guardian using automated GSM alerts.

## How It Works
The system operates on a **Detect Validate - Alert** logic to ensure accuracy and reduce "alert fatigue" for parents.

**1. Detection (The MQ Sensor**
  **The MQ Gas Sensor** samples the ambient air every **15 seconds.** It looks for the specific molecular concentrations of ethanol and natural gas.
 - **Threshold:** If the sensor reading exceeds a value of **500**, the local buzzer activates immediately.
   
**2. Validation**
   To prevent false alarms (e.g., from hand sanitizers or perfume), the system requires **three consecutive "High" readings** (totalling 45 seconds of exposure).
 -if the threat persists for 45 seconds, it is confirmed as a genuine hazard.
 
**3. False Alarm Mitigation (The 30-Minute Reset)**
   If the sensor detects "clean air (below 500), an internal time starts. If the air remains clean for **30 minutes,** the "Strike Counter" resets to zero, ensuring one-time environmental spikes don't trigger future alerts.
   
**4. Communication (GSM Module)**
   Once a threat is validated, the **SIM800L Module** automatically transmits a distress SMS to the pre-programmed guardian's mobile number.
   
If the sensor detects "clean air (below 500), an internal time starts. If the air remains clean for **30 minutes,** the "Strike Counter" resets to zero, ensuring one-time environmental spikes don't trigger future alerts.

### Features
- **Real-time Gas Sensing:** Utilizes the Mq Gas Sensor to monitor environmental air quality.
- **Intelligent Alert Logic:** Uses a "3-Strike" rule (3 rule consecutive  15-second detections) to confirm a threat before alerting.
- **Guardian Notification:** Integrated SIM800L GSM Module sends automated SMS alerts.
- **False Alarm Mitigation:** Automate 30-minute reset timer for temporary exposes (eg., hand sanitizer)
- **Future-Ready:** Development paths for GPS tracking and Heart Rate monitoring.
  

## User Instructions
1. Wear the SafetyConnect on your wrist.
2. Press and Hold the side button till display show
3. If gas and/or alcohol is detected, the buzzer will make noise and the LED will display warnings (Thrice). Hence, on the third time, Buzz and SMS Alert to Guardians.
4. If a gas leak is detected, buzz and LED flashes.

