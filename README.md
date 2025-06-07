🚧 Pothole Detection and Reporting System

Please read this for Jist/Summary of whole Project idea:

The basic idea of this project stems from a common issue in India: despite being entrusted with regional development, many politicians are unable to effectively address problems faced by the public—especially poor road conditions. On encountering potholes, people often think, "If only I could fix this myself." However, they lack the means to do so.

Our project, nexPave, which was among the top 8 shortlisted teams out of 400+ at a National Social Hackathon (from 63 teams that reached the Teach-Out round), offers a practical solution. Through our platform, users can visit the website and upload images of potholes. A machine learning model, trained on a Kaggle dataset, analyzes the image to predict the pothole’s severity, size, and suggests an estimated bounty for reporting it.

The report is then forwarded to a Contractor Dashboard, where registered contractors can log in and choose to fix the reported pothole. We’ve also implemented various verification mechanisms to ensure that the pothole has genuinely been fixed. The platform is thoughtfully designed to account for all possible human factors and ensure effective, community-driven road repair.


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
git clone (https://github.com/ftpulkit/projNexPave/)
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

🤝 Tanmay – Backend, REST APIs=


📜 License
This project is licensed under the MIT License – see the LICENSE file for details.
