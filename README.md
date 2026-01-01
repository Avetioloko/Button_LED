const int buttonPin = 2;   // кнопка
const int ledPin = 8;      // светодиод

void setup() {
  pinMode(buttonPin, INPUT_PULLUP); // кнопка с подтяжкой
  pinMode(ledPin, OUTPUT);
}

void loop() {
  int buttonState = digitalRead(buttonPin);

  if (buttonState == LOW) {   // кнопка нажата
    digitalWrite(ledPin, HIGH);
  } else {                    // кнопка не нажата
    digitalWrite(ledPin, LOW);
  }
}
Как это работает
