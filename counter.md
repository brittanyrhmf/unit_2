# Automatic 3-bit LED Binary counter 
![Image 17-11-2021 at 00 10](https://user-images.githubusercontent.com/89038847/142058395-039ec9ed-5d24-43e1-b1b4-42fdac2f136d.jpg)

// C++ code
//

int pin2 = 2;
int pin3 = 3;
int pin4 = 4;

void setup()
{
  pinMode(pin2, OUTPUT);
  pinMode(pin3, OUTPUT);
  pinMode(pin4, OUTPUT);
  
}


void loop()
{
  digitalWrite(pin2,LOW);
  digitalWrite(pin3,LOW);
  digitalWrite(pin4,LOW);
  delay(750);
  
  digitalWrite(pin2,LOW);
  digitalWrite(pin3,LOW);
  digitalWrite(pin4,HIGH);
  delay(750);
  
  digitalWrite(pin2,LOW);
  digitalWrite(pin3,HIGH);
  digitalWrite(pin4,LOW);
  delay(750);
  
  digitalWrite(pin2,LOW);
  digitalWrite(pin3,HIGH);
  digitalWrite(pin4,HIGH);
  delay(750);
  
  digitalWrite(pin2,HIGH);
  digitalWrite(pin3,LOW);
  digitalWrite(pin4,LOW);
  delay(750);
  
  digitalWrite(pin2,HIGH);
  digitalWrite(pin3,LOW);
  digitalWrite(pin4,HIGH);
  delay(750);
  
  digitalWrite(pin2,HIGH);
  digitalWrite(pin3,HIGH);
  digitalWrite(pin4,LOW);
  delay(750);
  
  digitalWrite(pin2,HIGH);
  digitalWrite(pin3,HIGH);
  digitalWrite(pin4,HIGH);
  delay(750);
  
  digitalWrite(pin2,LOW);
  digitalWrite(pin3,LOW);
  digitalWrite(pin4,LOW);
  delay(750);
  
  digitalWrite(pin2,LOW);
  digitalWrite(pin3,LOW);
  digitalWrite(pin4,HIGH);
  delay(750);
  
  digitalWrite(pin2,LOW);
  digitalWrite(pin3,HIGH);
  digitalWrite(pin4,LOW);
  delay(750);
  
  digitalWrite(pin2,LOW);
  digitalWrite(pin3,HIGH);
  digitalWrite(pin4,HIGH);
  delay(750);
  
  digitalWrite(pin2,HIGH);
  digitalWrite(pin3,LOW);
  digitalWrite(pin4,LOW);
  delay(750);
  
  digitalWrite(pin2,HIGH);
  digitalWrite(pin3,LOW);
  digitalWrite(pin4,HIGH);
  delay(750);
  
  digitalWrite(pin2,HIGH);
  digitalWrite(pin3,HIGH);
  digitalWrite(pin4,LOW);
  delay(750);
  
  digitalWrite(pin2,HIGH);
  digitalWrite(pin3,HIGH);
  digitalWrite(pin4,HIGH);
  
}

# 3-bit LED binary counter w/ buttons
<img width="717" alt="Screenshot 2021-11-23 at 06 45 09" src="https://user-images.githubusercontent.com/89038847/142964234-7612722f-2df0-4116-9258-9c808cefd7a5.png">


// C++ code

int pin2 = 2;
int pin3 = 3;
int pin4 = 4;

//variables buttons
int button2 = 2;
int button3 = 3;
int button4 = 4;

//variables state of button
int buttonState2 = 0;
int buttonState3 = 0;
int buttonState4 = 0;

void setup()
{
	pinMode(button2, INPUT);
  	pinMode(button3, INPUT);
  	pinMode(button4, INPUT);
    pinMode(pin2, OUTPUT);
  	pinMode(pin3, OUTPUT);
  	pinMode(pin4, OUTPUT);
}


void loop()
{	
  //check if button is pushed
  	buttonState2 = digitalRead(button2);
    if (buttonState2 == HIGH)
    {
    	digitalWrite(pin2, HIGH);
  	} 
  	else{
    	digitalWrite(pin2, LOW);
  	}
  
  	buttonState3 = digitalRead(button3);
    if (buttonState3 == HIGH)
    {
    	digitalWrite(pin3, HIGH);
  	} 
  	else{
    	digitalWrite(pin3, LOW);
  	}
  
  	buttonState4 = digitalRead(button4);
    if (buttonState4 == HIGH)
    {
    	digitalWrite(pin4, HIGH);
  	} 
  	else{
    	digitalWrite(pin4, LOW);
  	}
    
}
