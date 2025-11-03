### Microbit Code to Receive the Data from AI Vision App

[Open in MakeCode Editor](https://makecode.microbit.org/_AFw19V4gXaRL)

<img width="800" height="600" alt="image" src="https://github.com/user-attachments/assets/2bc526df-7fe9-4f5e-a1ce-767aff1e9dec" />

---

### Arduino Code to Receive the Data from AI Vision App

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
