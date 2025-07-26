# Airport-Info-API-Node.js-Express-and-TypeScript-Project

🔰 Project Summary
This project is a simple REST API built with Node.js, Express, and TypeScript, designed to provide information about airports based on their IATA codes. It mimics real-world backend development scenarios like querying a data source and returning JSON responses to client requests.

🚀 Features
Built using Express.js and TypeScript

Returns airport information (code, name, city, country)

Uses a pre-defined dataset (airportData.ts)

Validates query parameters

Error handling for missing or invalid airport codes

Easily extendable for future DB integration

🏁 Project Start Point
Initialize Node.js project

bash
Copy
Edit
npm init -y
Install required packages

bash
Copy
Edit
npm install express
npm install --save-dev typescript ts-node @types/node @types/express
Create tsconfig.json

bash
Copy
Edit
npx tsc --init
Set up basic folder structure:

bash
Copy
Edit
/src
  ├── data-source.ts
  ├── airportData.ts
  ├── index.ts
  └── entity/
       ├── Airport.ts
       ├── City.ts
       └── Country.ts
Add airport data and define routes

🛑 Project End Point
Server runs successfully on http://localhost:3000

You can access:

Root route: GET /

json
Copy
Edit
Hello from Airport Info API!
Airport info route: GET /api/airport-info?code=DEL

json
Copy
Edit
{
  "code": "DEL",
  "name": "Indira Gandhi International Airport",
  "city": "Delhi",
  "country": "India"
}
Supports multiple airport queries by changing the IATA code

Code structure is modular and ready for production-level extension

🛠 Localhost Setup in VS Code
To run this project locally using VS Code:

Open terminal in VS Code

Run the dev server:

bash
Copy
Edit
npx ts-node src/index.ts
Open browser and test on http://localhost:3000/api/airport-info?code=DEL

📂 How to Push to GitHub
Initialize git:

bash
Copy
Edit
git init
git add .
git commit -m "Initial commit - Airport Info API"
Push to GitHub:

bash
Copy
Edit
git remote add origin https://github.com/06318Ganesh/airport-info-api.git
git branch -M main
git push -u origin main
