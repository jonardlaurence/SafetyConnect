# SafetyConnect Wristband

## Project Overview:  
is a discreet, wearable, and protective wristband that detects alcohol and gas leaks that alerts the user and their parents and/or guardian. Unlike reactive seafety measures, this wristband autonomously detects environmental hazards specifically **Alcohol (Ethanol)** and **Natural Gas** and bridges the communication gap between a minor and their guardian using automated GSM alerts.

## How IT Works
The system operates on a **Detect Validate - Alert** logic to ensure accuracy and reduce "alert fatigue" for parents.
**1. Detection (The MQ Sensor**
**The MQ Gas Sensor** samples the ambient air every **15 seconds.** It looks for the specific molecular concentrations of ethanol and natural gas.
 - **Threshold:** If the sensor reading exceeds a value of **500**, the local buzzer activates immidiately..

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

