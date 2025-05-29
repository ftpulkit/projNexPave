🚧 Pothole Detection and Reporting System

Please read this for Jist/Summary of whole Project idea:

The basic idea of this project is that in our India, major bodies like politicians who are given responsibility of their region for development of it, are somehow not able to solve problems public face which is of roads. On going to any road, people critisize and think ki God, if  i was to be able to fix it i would have. But no souce for them to fix it. So finally my project nexPave which stood in a National Social Hackathon and was and top 8 of shortlisted 63 teach out of 400+teams came up with a Solution. Any user and visit our website and upload pothole image and ML model (trained locally from dataset available on Kaggle) will predict severity, size,etc of that pothole and tell an estimated bounty for reporting it. Further it goes to Contractor Dashboard where contractor can login into the page and opt to fix the pothole. Various verification to check f pothole is fixed is put too. 
Considering all human possibilities, the platform is designed.
![DashBoard of the website made](https://github.com/user-attachments/assets/7968a520-f2af-4cb4-b1ee-826894db9451)
![Contractor Dashboard](https://github.com/user-attachments/assets/a162df31-7048-48f9-b60c-bc4d7ac8ccd3)


🛠️ Tech Stack
Frontend	Backend	Other
React + TailwindCSS	Spring Boot (Java)	Mapbox API
ShadCN/UI	RESTful APIs	Multipart File Upload
Framer Motion	OpenAI (optional)	Google Maps (alternative)


An intelligent web-based system for real-time pothole detection, severity analysis, and reporting using AI. Citizens can report potholes with location, images, and details. The system provides estimated pothole size, severity, traffic flow impact, and assigns bounty rewards — all backed by a Spring Boot REST API and a React frontend.📸 Features
🌍 Location tagging using Mapbox
The Project made us stand among the top 10 of 63 teams shortlisted from 400+ teams in Social Hackathon- An National Hackathon
📷 Image upload with real-time preview

🧠 AI-based analysis (Severity, Size, Traffic Flow)

💰 Dynamic bounty generation

📈 Success dashboard with all details

⚙️ Spring Boot API backend

☁️ Global accessibility (ESP32-compatible architecture ready for IoT)
🛠️ Tech Stack
Frontend	Backend	Other
React + TailwindCSS	Spring Boot (Java)	Mapbox API
ShadCN/UI	RESTful APIs	Multipart File Upload
Framer Motion	OpenAI (optional)	Google Maps (alternative)

🚀 Getting Started
📦 Clone the repository
bash
git clone https://github.com/yourusername/pothole-reporting-system.git
cd pothole-reporting-system

🧩 Frontend Setup
bash
cd frontend
npm install
npm start

⚙️ Backend Setup
bash
cd backend
./mvnw spring-boot:run

Configure your application.properties:
properties

spring.servlet.multipart.max-file-size=10MB
spring.servlet.multipart.max-request-size=10MB
spring.cors.allowed-origins=http://localhost:3000
📡 API Endpoints
Method	Endpoint	Description
POST	/api/report	Uploads pothole report and returns analysis
GET	/api/reports	Get all pothole reports (admin)

📊 AI Output Fields
Severity → Low, Moderate, Severe

Estimated Size → e.g., 58cm x 34cm

Traffic Flow → Light, Moderate, Heavy

Bounty → ₹ based on severity and traffic

📁 Project Structure
bash
/backend
 └── src/main/java/com/pothole/...
     ├── controllers
     ├── services
     ├── models
     └── repositories

/frontend
 ├── src/
 │   ├── components/
 │   ├── App.tsx
 │   └── index.tsx
 └── public/
🧪 Sample JSON Response
json
{
  "severity": "Moderate",
  "estimatedSize": "58 cm x 34 cm",
  "trafficFlow": "Heavy",
  "bounty": 1400
}
✨ Contributors
👨‍💻 Pulkit – Frontend, AI Integration

🤝 Tanmay – Backend, REST APIs
![Dashboard](https://github.com/user-attachments/assets/809802f8-6a53-4dd7-af7c-d6b259c1b7c5)


📜 License
This project is licensed under the MIT License – see the LICENSE file for details.
