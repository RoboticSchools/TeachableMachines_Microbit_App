```C++

void setup() {
  Serial.begin(115200);
}

void loop() {
  if (Serial.available()) {
    String data = Serial.readStringUntil('\n');
    data.trim();
    Serial.println(data);
  }
}


```
