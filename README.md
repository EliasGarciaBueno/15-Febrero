# 15-Febrero
int j;
int verde = 13;
int rojo = 7;
int amarillo = 2;
int a;
int b;
int c;
int k;
int y;


void setup() {
  pinMode(verde, OUTPUT);
  pinMode(rojo, OUTPUT);
  pinMode(amarillo, OUTPUT);
 Serial.begin (9600);
 Serial.println("¿Cuántas veces quieres que prenda el led verde?");
  delay(4000);
  a = Serial.parseInt ();
 Serial.println("¿Cuántas veces quieres que prenda el led rojo?");
  delay(4000);
  b = Serial.parseInt ();
 Serial.println("¿Cuántas veces quieres que prenda el led amarillo?");
  delay(4000);
  c = Serial.parseInt ();
}


void loop() {
  for(int i = 0; i<a; i++){
  digitalWrite(verde, HIGH);
  delay(500);
  digitalWrite(verde, LOW);
  delay(500);
}
 for(int i = 0; i<b; i++){
  digitalWrite(rojo, HIGH);
  delay(500);
  digitalWrite(rojo, LOW);
  delay(500);
}
  
 for(int i = 0; i<c; i++){
  digitalWrite(amarillo, HIGH);
  delay(500);
  digitalWrite(amarillo, LOW);
  delay(500);
 }


  
  // put your main code here, to run repeatedly:

}
