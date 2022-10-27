#  roleta de led

int botao1 = 13, botao2 = 12;
  int ledazul = 3;
  int ledamarelo = 4;
int ledvermelho = 5;

void setup()
{ 
   
  
  pinMode(botao1, INPUT_PULLUP);
  pinMode(ledazul, OUTPUT);
  digitalWrite(ledazul, LOW);
  pinMode(ledazul, OUTPUT);
  digitalWrite (ledamarelo, LOW);
  pinMode(ledazul, OUTPUT);
  digitalWrite(ledvermelho, LOW);
}

void loop()
{
  digitalWrite(ledazul, HIGH);
  delay(1000); 
  digitalWrite(ledazul,LOW);
  
  digitalWrite(ledamarelo, HIGH);
  delay(1000);
  digitalWrite(ledamarelo, LOW);
  
  digitalWrite(ledvermelho, HIGH);
  delay(1000);
  digitalWrite(ledvermelho, LOW);
}
