🎧 SPCUBE – Cloud-Powered Music Subscription App

Welcome to SPCUBE – a fully functional music subscription web app built entirely on AWS.
This project is designed to help users search, subscribe, and manage their favorite music
in a modern, serverless architecture.

It’s more than just a tech project — it’s a personal cloud engineering adventure 🎯.

🌐 Live Features

- 🔐 User Login & Registration
- 🎵 Song Search (by title, artist, album, year)
- ❤️ Subscribe/Unsubscribe to your favorite tracks
- 🖼️ Artist Images fetched from S3 using presigned URLs
- ☁️ Fully serverless backend using Lambda + API Gateway + DynamoDB
- 🖥️ Frontend hosted on EC2 with a clean, Spotify-style UI

🧱 Built With

Layer         | Technology
------------- | -------------------------
Frontend      | HTML, CSS, JavaScript
Backend       | AWS Lambda (Python)
API Gateway   | REST API integration
Database      | DynamoDB
Storage       | Amazon S3 (presigned URLs)
Hosting       | EC2 (Apache2 on Ubuntu)

🚀 Quick Start Guide

1. Clone the Repo
   git clone https://github.com/your-username/spcube-music-app.git
   cd spcube-music-app

2. Create DynamoDB Tables
   python create_music_table.py
   python create_subscription_table.py

3. Upload Music Data
   python load_music_data.py

4. Upload Artist Images to S3
   python upload_artist_images.py

5. Launch EC2 & Set Up Web Server
   - Install Apache2 on Ubuntu EC2
   - Copy HTML files to /var/www/html/

6. Deploy Lambda Functions
   - Set up REST endpoints via API Gateway
   - Link each action (login, register, subscribe, etc.) to respective Lambda

7. Update API URLs in HTML
   - Make sure frontend calls correct API Gateway endpoints

📁 Project Structure

SPCUBE_MusicApp/
├── create_music_table.py
├── create_subscription_table.py
├── load_music_data.py
├── upload_artist_images.py
├── createbucket.py
├── login.html
├── register.html
├── main.html

💡 Ideas for Future Enhancement

- 🎙️ Add audio previews
- 📊 Analytics dashboard
- 👤 User profile page
- 🔒 JWT-based auth

👋 Author

Puneeth  
Cloud & Data Enthusiast | Data Scientist
LinkedIn: https://www.linkedin.com/in/puneethkrishna-b-79a5b71a3/


Thanks for checking out SPCUBE! ⭐
