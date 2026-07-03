# codealpha_task-2
### Sensor-Based Simulation
Project: Temperature-Based LED Control using Arduino and Tinkercad

**Components Used:**
- Arduino Uno
- TMP36 Temperature Sensor

**Working:**
- Reads temperature using TMP36 sensor.
- If temperature exceeds threshold, built-in LED turns ON.
- Otherwise LED remains OFF.

**Code:**
```cpp
int sensorPin = A0;
int sensorValue = 0;

void setup() {
  pinMode(13, OUTPUT);
  Serial.begin(9600);
}

void loop() {
  sensorValue = analogRead(sensorPin);

  if (sensorValue > 150) {
    digitalWrite(13, HIGH);
  } else {
    digitalWrite(13, LOW);
  }

  delay(500);
}
```
<img width="1352" height="630" alt="Screenshot_2-7-2026_143944_www tinkercad com" src="https://github.com/user-attachments/assets/cbbc9e08-2012-44fd-903b-ef0d195007de" />
<img width="1350" height="634" alt="Screenshot_2-7-2026_144040_www tinkercad com" src="https://github.com/user-attachments/assets/ef3ee86e-7150-4a3b-9791-1481d84826b8" />
<img width="1351" height="632" alt="Screenshot_2-7-2026_144118_www tinkercad com" src="https://github.com/user-attachments/assets/aa397576-6f9e-40e1-9791-0bd3af87ea48" />
<img width="1358" height="633" alt="Screenshot_2-7-2026_144157_www tinkercad com" src="https://github.com/user-attachments/assets/b1e30fe4-6834-497c-a65e-6946cbebf787" />

    
