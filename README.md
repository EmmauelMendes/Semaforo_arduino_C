# Semaforo_arduino_C
int tempo = 0;

int counter;

void setup()
{
  pinMode(8, OUTPUT);
  pinMode(5, OUTPUT);
  pinMode(2, OUTPUT);
  pinMode(13, OUTPUT);
  pinMode(12, OUTPUT);
  pinMode(10, OUTPUT);
  pinMode(11, OUTPUT);
  pinMode(9, OUTPUT);
  pinMode(7, OUTPUT);
  pinMode(6, OUTPUT);
  pinMode(4, OUTPUT);
  pinMode(3, OUTPUT);
}

void loop()
{
  for (counter = 0; counter < 10; ++counter) {
    digitalWrite(8, HIGH);
    digitalWrite(5, HIGH);
    digitalWrite(2, HIGH);
    digitalWrite(13, HIGH);
    delay(5000);
    digitalWrite(13, LOW);
    digitalWrite(12, HIGH);
    digitalWrite(5, HIGH);
    digitalWrite(2, HIGH);
    delay(5000); 
    digitalWrite(10, HIGH);
    digitalWrite(2, HIGH);
    digitalWrite(11, HIGH);
    digitalWrite(12, LOW);
    digitalWrite(8, LOW);
    delay(5000);
    digitalWrite(10, LOW);
    digitalWrite(9, HIGH);
    digitalWrite(2, HIGH);
    digitalWrite(11, HIGH);
    digitalWrite(12, LOW);
    delay(5000); 
    digitalWrite(9, LOW);
    digitalWrite(2, HIGH);
    digitalWrite(11, HIGH);
    digitalWrite(12, LOW);
    digitalWrite(7, HIGH);
    digitalWrite(8, HIGH);
    digitalWrite(5, LOW);
    delay(5000); 
    digitalWrite(6, HIGH);
    digitalWrite(2, HIGH);
    digitalWrite(11, HIGH);
    digitalWrite(7, LOW);
    digitalWrite(8, HIGH);
    digitalWrite(5, LOW);
    delay(5000);
    digitalWrite(6, LOW);
    digitalWrite(2, LOW);
    digitalWrite(11, HIGH);
    digitalWrite(8, HIGH);
    digitalWrite(5, HIGH);
    digitalWrite(4, HIGH);
    delay(5000); 
    digitalWrite(2, LOW);
    digitalWrite(11, HIGH);
    digitalWrite(8, HIGH);
    digitalWrite(5, HIGH);
    digitalWrite(4, HIGH);
    delay(5000); 
    digitalWrite(11, HIGH);
    digitalWrite(8, HIGH);
    digitalWrite(5, HIGH);
    digitalWrite(4, LOW);
    digitalWrite(3, HIGH);
    delay(5000); 
    digitalWrite(11, HIGH);
    digitalWrite(8, HIGH);
    digitalWrite(5, HIGH);
    digitalWrite(4, LOW);
    digitalWrite(3, LOW);
  }
}
