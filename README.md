# Progam-Arduino
int botao1 = 13, botao2 = 3;
int led = 7;
int contador = 0;


void setup()
{
  pinMode (led, OUTPUT);
  pinMode (botao1, INPUT_PULLUP);
  pinMode (botao2, INPUT_PULLUP);
}

void loop ()
{
  if (digitalRead(botao1)== LOW){
    contador = 1;
    delay(1000);
  }
  
  if (digitalRead(botao2)== LOW){
    contador=0;
    delay(1000);
  }
  
  if (contador == 1){;
    digitalWrite(led,HIGH);
  }
 
    
    if (contador == 0){;
       digitalWrite (led,LOW);
                      }
                       
    if (contador == 2){;
       digitalWrite(led,HIGH);
                      }
     if (contador == 0){;
        digitalWrite (led,LOW);
    
    
  }
  
}
