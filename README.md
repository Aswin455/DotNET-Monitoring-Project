
# DotNET Monitoring Dashboard

A real-time system monitoring dashboard developed using ASP.NET Core (.NET 8). The application provides live monitoring of CPU usage, memory utilization, system information, and weather data through a web-based interface.

This project demonstrates system diagnostics, REST API integration, configuration management, and ASP.NET Core MVC application development.

---

# Features

* Real-time CPU monitoring
* Memory usage tracking
* System information dashboard
* Weather API integration
* CPU load simulation tools
* Error testing utilities
* Responsive web interface
* ASP.NET Core MVC architecture

---

# Technology Stack

| Technology              | Purpose                  |
| ----------------------- | ------------------------ |
| ASP.NET Core (.NET 8)   | Backend Framework        |
| C#                      | Programming Language     |
| Razor Pages / MVC       | Frontend Rendering       |
| OpenWeather API         | Weather Data Integration |
| HTML / CSS / JavaScript | User Interface           |
| Git & GitHub            | Version Control          |

---

# Project Structure

```bash id="p1"
DotNET-Monitoring-Project-main/
│
├── src/
│   ├── Controllers/
│   ├── Models/
│   ├── Services/
│   ├── Views/
│   ├── wwwroot/
│   ├── appsettings.json
│   ├── Program.cs
│   └── DotNET-Monitoring.csproj
│
└── README.md
```

---

# Application Modules

## Home

Landing page of the application.

## System Information

Displays:

* Operating system details
* CPU information
* RAM statistics
* Host system information

## Monitoring Dashboard

Provides:

* Live CPU usage
* Memory utilization monitoring
* Real-time system statistics

## Weather

Displays live weather information using OpenWeather API integration.

## Tools

Provides:

* CPU stress testing
* Error simulation utilities

---

# Screenshots

## Home Page

```text id="p2"
images/home.png
```

## System Information Dashboard

```text id="p3"
images/info.png
```

## Monitoring Dashboard

```text id="p4"
images/monitor.png
```

## Weather Dashboard

```text id="p5"
images/weather.png
```

## Tools and Diagnostics

```text id="p6"
images/tools.png
```

---

# Prerequisites

* macOS Terminal
* Homebrew
* Git
* .NET SDK 8

---

# Installation and Setup

## Clone Repository

```bash id="p7"
mkdir my-project && cd my-project

git clone https://github.com/your-username/DotNET-Monitoring-Dashboard.git

cd DotNET-Monitoring-Dashboard
```

---

# Install Git

```bash id="p8"
brew install git
```

---

# Install .NET SDK 8

```bash id="p9"
brew install --cask dotnet-sdk@8
```

Verify installation:

```bash id="p10"
dotnet --version
```

Expected output:

```text id="p11"
8.0.x
```

---

# Navigate to Source Directory

```bash id="p12"
cd src
```

---

# Configure Weather API

Open configuration file:

```bash id="p13"
nano appsettings.json
```

Replace:

```json id="p14"
"ApiKey": "YOUR_API_KEY_HERE"
```

with:

```json id="p15"
"ApiKey": "YOUR_REAL_API_KEY"
```

Generate API key from:

[OpenWeather API Platform](https://openweathermap.org/api?utm_source=chatgpt.com)

Save file:

```text id="p16"
CTRL + O
ENTER
CTRL + X
```

---

# Run the Application

```bash id="p17"
dotnet run
```

If port 5000 is already in use:

```bash id="p18"
dotnet run --urls=http://localhost:5050
```

---

# Access the Application

Open browser:

```text id="p19"
http://localhost:5000
```

or

```text id="p20"
http://localhost:5050
```

---

# Important Commands

## Restore Dependencies

```bash id="p21"
dotnet restore
```

---

## Build Project

```bash id="p22"
dotnet build
```

---

## Run Project

```bash id="p23"
dotnet run
```

---

## Run with Hot Reload

```bash id="p24"
dotnet watch run
```

---

## Clean Project

```bash id="p25"
dotnet clean
```

---

## List Installed SDKs

```bash id="p26"
dotnet --list-sdks
```

---

## List Installed Runtimes

```bash id="p27"
dotnet --list-runtimes
```

---

## Check Running Process on Port

```bash id="p28"
lsof -i :5000
```

---

## Kill Process Using Port

```bash id="p29"
kill -9 $(lsof -t -i:5000)
```

---

# Docker Support

## Build Docker Image

```bash id="p30"
docker build -t dotnet-monitoring-app .
```

---

## Run Docker Container

```bash id="p31"
docker run -p 5000:5000 dotnet-monitoring-app
```

---

# Common Issues

## Port Already in Use

Error:

```text id="p32"
Address already in use
```

Solution:

```bash id="p33"
kill -9 $(lsof -t -i:5000)
```

---

## Weather API Unauthorized

Possible causes:

* Invalid API key
* API key not activated
* Incorrect API configuration

Solution:

* Update `appsettings.json`
* Restart application
* Wait a few minutes after generating API key

---

## .NET SDK Not Found

Verify installation:

```bash id="p34"
dotnet --version
```

---

# Learning Outcomes

* ASP.NET Core MVC application development
* REST API integration
* Real-time monitoring concepts
* JSON configuration management
* Cross-platform .NET development
* System diagnostics and monitoring

---

# Future Improvements

* Authentication and authorization
* Database integration
* Historical monitoring analytics
* Docker Compose support
* Kubernetes deployment
* Cloud deployment on Azure
* Prometheus and Grafana integration

---

# Author

Developed as part of a .NET monitoring and cloud-native application learning project.

---

# License

This project is intended for educational and learning purposes.

