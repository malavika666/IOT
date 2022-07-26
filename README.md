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
