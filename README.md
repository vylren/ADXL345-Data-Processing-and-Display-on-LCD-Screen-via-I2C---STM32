[EN]

This repository contains code for interfacing with the ADXL345 accelerometer sensor and processing the data obtained from it. The main goal of this project is to demonstrate how to acquire, process, and visualize sensor data in an embedded system environment.
Repository includes libraries which are needed for both, OLED and LCD displays. i2c-lcd drivers ensure that the output is transmitted to your LCD display via I2C communication protocol. Whereas ssd1306 is dedicated to OLED displays. It is up for each user individually to customize and adapt functions of the code. 

**Features:**

-Sensor Initialization: The code initializes the ADXL345 sensor, configuring it for data acquisition. <br />
-Data Acquisition: Utilizing I2C communication protocol, the code reads raw acceleration data from the ADXL345 sensor. <br />
-Data Processing: The raw sensor data is processed to calculate RMS values for each axis, providing a measure of the root mean square acceleration. <br />
-Visualization: The processed data is visualized on an LCD screen, providing real-time feedback on the acceleration values in each axis. The refresh rate can be customized according to your needs by calibrating TIM6 and TIM7. <br />
-UART Transmission: The processed data is transmitted via UART communication for external monitoring or logging purposes.

**Setup:**

-Hardware Setup: Connect the ADXL345 sensor to the microcontroller board according to the provided pinout.<br />
-Software Setup: Import the provided code into your development environment, ensuring all necessary dependencies are included.

**Usage:**

-Initialize the sensor by calling the adxl_init() function.<br />
-Start data acquisition and processing by running the main loop.<br />
-Visualize the processed data on the connected LCD screen.<br />
-Optionally, monitor or log the data transmitted via UART for further analysis.

[LT]

Šioje saugykloje yra kodas (bei visi reikalingi failai), skirtas sąveikai su ADXL345 akselerometro jutikliu ir iš jo gautų duomenų apdorojimui. Pagrindinis šio projekto tikslas - parodyti, kaip gauti, apdoroti ir vizualizuoti jutiklio duomenis įterptinės sistemos aplinkoje.
Į saugyklą įtrauktos bibliotekos, reikalingos tiek OLED, tiek LCD ekranams. i2c-lcd tvarkyklės užtikrina, kad išvestis į LCD ekraną būtų perduodama I2C ryšio protokolu. O ssd1306 skirta OLED ekranams. Kiekvienas naudotojas gali individualiai pritaikyti ir panaudoti kodo funkcijas. 

**Funkcijos:**

-Jutiklio inicijavimas: Kodas inicializuoja ADXL345 jutiklį, sukonfigūruoja jį duomenų rinkimui.<br />
-Duomenų gavimas: Kodas, naudodamas I2C ryšio protokolą, nuskaito neapdorotus pagreičio duomenis iš ADXL345 jutiklio.<br />
-Duomenų apdorojimas: Neapdoroti jutiklio duomenys apdorojami, kad būtų apskaičiuotos kiekvienos ašies vidutinės kvadratinės vertės ir taip nustatytas vidutinis kvadratinis pagreitis.<br />
-Vizualizavimas: Apdoroti duomenys vizualizuojami LCD ekrane, realiuoju laiku pateikiant grįžtamąjį ryšį apie kiekvienos ašies pagreičio vertes. Atnaujinimo dažnį galima pritaikyti pagal savo poreikius kalibruojant TIM6 ir TIM7.<br />
-UART perdavimas: Apdoroti duomenys perduodami UART ryšiu, kad juos būtų galima stebėti iš personalinio kompiuterio arba registruoti.

**Nustatymas:**

-Techninės įrangos nustatymas: ADXL345 jutiklį prie mikrovaldiklio plokštės prijunkite pagal pateiktą kontaktų išdėstymą.<br />
-Programinės įrangos sąranka: Importuokite pateiktą kodą į savo kūrimo aplinką ir įsitikinkite, kad įtrauktos visos būtinos bibliotekos.

**Panaudojimas**

-Inicializuokite jutiklį iškviesdami funkciją adxl_init().<br />
-Pradėkite duomenų rinkimą ir apdorojimą paleisdami pagrindinį ciklą.<br />
-Vizualizuokite apdorotus duomenis prijungtame LCD ekrane.<br />
-Pasirinktinai stebėkite arba registruokite UART perduodamus duomenis tolesnei analizei.
