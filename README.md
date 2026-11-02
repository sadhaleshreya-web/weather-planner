\# Daily Weather \& Outfit Planner



A lightweight Java command-line utility that fetches daily weather forecasts, analyzes current conditions, and provides a morning briefing telling you what to wear and what gear to bring.



\---



\## Project Goal \& Overview

To eliminate morning guesswork by automatically pulling local weather data and translating temperature, precipitation, wind, and UV indexes into actionable clothing and accessory recommendations.



\---



\## How It Works



This software connects to the Open-Meteo REST API using standard Java libraries to retrieve live daily weather data. It parses weather metrics (temperature, precipitation, wind speed, UV index) and feeds them into a rule engine that matches weather thresholds to appropriate clothing items and gear (e.g., umbrellas, sunglasses). Finally, it outputs a clean morning briefing summary to the terminal.



\### System Architecture Diagram

\\`\\`\\`

![System Diagram](docs/diagram.png)

\\`\\`\\`



\---



\## Tech Stack



\- \*\*Language:\*\* Java (JDK 17+)

\- \*\*Libraries:\*\* \\`java.net.http\\` (Built-in HTTP Client), \\`java.util\\`

\- \*\*External tools / APIs:\*\* \[Open-Meteo API](https://open-meteo.com/) (Public, free API - no API key required)



\---



\## Setup



1\. \*\*Clone the repository:\*\*

&#x20;  \\`\\`\\`bash

&#x20;  git clone https://github.com/sadhaleshreya-web/weather-planner.git

&#x20;  cd weather-planner

&#x20;  \\`\\`\\`



2\. \*\*Verify Java Installation (JDK 17+ required):\*\*

&#x20;  \\`\\`\\`bash

&#x20;  java -version

&#x20;  \\`\\`\\`



3\. \*\*Compile the source code:\*\*

&#x20;  \\`\\`\\`bash

&#x20;  javac -d bin src/main/java/com/weather/Main.java

&#x20;  \\`\\`\\`



\---



\## Usage



Run the compiled application from your terminal:



\\`\\`\\`bash

java -cp bin com.weather.Main

\\`\\`\\`



\*\*Sample Output:\*\*

\\`\\`\\`text

Fetching weather data...



\--- MORNING BRIEFING ---

Temperature: 65°F (Mild)

Outfit: Wear a light jacket and jeans.

Gear Warning: UV Index is high (6.5) - Don't forget your sunglasses!

\\`\\`\\`



\---



\## Roadmap



Features planned for future iterations (derived from Quadrant 2: Schedule of the Eisenhower Matrix):



\- \[ ] Native OS desktop notifications for daily morning alerts

\- \[ ] Automated daily briefing triggers via OS Task Scheduler or cron

\- \[ ] User configuration file (\\`config.properties\\`) for custom location coordinates and temperature thresholds

\- \[ ] Support for multi-city location profiles



\---



\## Eisenhower Matrix



\- \*\*DO (MVP Scope):\*\* Open-Meteo API integration, raw data parser, basic temperature/rain rule engine, formatted console output.

\- \*\*SCHEDULE (Roadmap):\*\* Desktop notifications, automated daily cron execution, custom user config file.

\- \*\*DELEGATE (Libraries):\*\* Built-in \\`java.net.http\\` for network requests.

\- \*\*DELETE (Cut):\*\* 3D weather radar graphics, user account/login system, social sharing features.



\---



\## Author



\- \*\*Shreya Sadhale\*\* - \[sadhaleshreya-web](https://github.com/sadhaleshreya-web)

"@

