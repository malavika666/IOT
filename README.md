# IOT
LED:<br>
https://wokwi.com/projects/334908784155558482<br>
3 LED:<br>
https://wokwi.com/projects/334909797910446674<br>
RGB: <br>
https://wokwi.com/projects/335704197045420626<br>
LCD:<br>
https://wokwi.com/projects/334973183140561490<br>
SERVO:<br>
https://wokwi.com/projects/334977644162450004<br>website:( https://www.instructables.com/Arduino-Servo-Motors/)<br>
servo Motor(for loop)
:https://wokwi.com/projects/334979679252382290<br>
Servomotor using sliding potentiometer:<br> 
https://wokwi.com/projects/334981596299919955<br>
Servomotor using Pushbutton:<br>
https://wokwi.com/projects/335700050397102675<br>
Buzzer:<br>
https://wokwi.com/projects/335065567075500626<br>
Buzzer using Pushbutton:<br>
https://wokwi.com/projects/335068762405339732<br>
Ultrasonic Sensor:<br> 
https://wokwi.com/projects/335071514961379924<br>
Ultrasonic sensor with buzzer: <br> 
https://wokwi.com/projects/335073425483629139<br>
Ultrasonis sensor,buzzer with led:<br>
https://wokwi.com/projects/335612307321127508<br>
Buzzer with LED and Pushbutton : <br>
https://wokwi.com/projects/335699245817397844<br>
Potentiometer with LED:  <br>        
https://wokwi.com/projects/335703563856511572
<br>
DHT22(humidity and temperature sensor):<br>
https://wokwi.com/projects/337602706761843283<br>
DHT22(humidity and temperature sensor)+LCD:<br>
https://wokwi.com/projects/337605674947052115
LED CHASER:
<br>
https://wokwi.com/projects/340774447162065491<br>
LDR:<br>
https://wokwi.com/projects/340776924078932564<br>
LDR+LED:<br>
https://wokwi.com/projects/340780293574099539<br>
IR+LED:<br>
https://wokwi.com/projects/340780454732890706<br>

ESP32:

LED
https://wokwi.com/projects/340882948429447764

3 LED:
https://wokwi.com/projects/340883307366449747

RGB LED
https://wokwi.com/projects/340883668203471443

LCD:
https://wokwi.com/projects/340883919581741650

Servomotor+Pushbutton:
https://wokwi.com/projects/340884422706332242

Sermotor+Slide Potentiometer:
https://wokwi.com/projects/340885196981142100

Buzzer+PushButton:
https://wokwi.com/projects/340885865271132754

Ultrasonicsensor+Buzzer:
https://wokwi.com/projects/340887871916343891

Potentiometer+LED:
https://wokwi.com/projects/340892222981407316

 LDR_LED< br>

 int ldr=A0;//Set A0(Analog Input) for LDR.< br>
 int value=0;< br>
 int led=D1;< br>
 void setup() {< br>
 Serial.begin(9600);< br>
 pinMode(led,OUTPUT);< br>
 }< br>

 void loop() {< br>
 value=analogRead(ldr);//Reads the Value of LDR(light).< br>
 Serial.println("LDR value is :");//Prints the value of LDR to Serial Monitor.< br>
 Serial.println(value);< br>
 if(value<50)< br>
   {
     digitalWrite(led,HIGH);//Makes the LED glow in Dark.< br>
   }< br>
   else< br>
   {< br>
     digitalWrite(led,LOW);//Turns the LED OFF in Light.< br>
   }< br>
   delay(1000);< br>
 }\< br>

   
ESP32:<br>
https://wokwi.com/projects/336966836274856532<br>
https://wokwi.com/projects/336968045044957778<br>

DHT11:
        #include <Adafruit_Sensor.h><br>
        #include <DHT.h>;<br>
        #define DHTPIN D7    // what pin we're connected to<br>
        #define DHTTYPE DHT11   // DHT 22  (AM2302)<br>
        DHT dht(DHTPIN, DHTTYPE); //// Initialize DHT sensor for normal 16mhz Arduino<br>
       //Variables<br>
       int chk;
       float hum;  //Stores humidity value<br>
       float temp; //Stores temperature value<br>
       void setup()<br>
       {<br>
       Serial.begin(9600);<br>
       dht.begin();<br>
       }<br>
      void loop()<br>
     {<br>
       delay(2000);<br>
       //Read data and store it to variables hum and temp<br>
       hum = dht.readHumidity();<br>
       temp= dht.readTemperature();<br>
       //Print temp and humidity values to serial monitor<br>
       Serial.print("Humidity: ");<br>
       Serial.print(hum);<br>
       Serial.print(" %, Temp: ");<br>
       Serial.print(temp);<br>
       Serial.println(" Celsius");<br>
       delay(1000); //Delay 2 sec.<br>
   }<br>
https://randomnerdtutorials.com/esp8266-nodemcu-hc-sr04-ultrasonic-arduino/<br>

