# flask-gif-app
A simple Flask web application that displays a random fun GIF on each refresh. The app is containerized using Docker and runs on port 80.

**Demo**

Displays a new random GIF every time you refresh the browser.

Perfect for lightweight testing or just for fun!

**Technologies Used**

Python 3.10+

Flask (for web server)

HTML/CSS (via Jinja templates)

Docker (for containerization)

**Folder Structure**

graphql
Copy
Edit
flask-gif-app/
├── app.py               # Main Flask application
├── Dockerfile           # Docker build file
├── requirements.txt     # Python dependencies
├── docker-setup.sh      # Optional setup script
└── templates/
    └── index.html       # HTML template for GIF display
    
**How to Build & Run the App**

Clone the Repository

bash
Copy
Edit
git clone https://github.com/example-user/flask-gif-app.git
cd flask-gif-app

**Build the Docker Image**

bash
Copy
Edit
docker build -t flask-gif-app 

**Run the Docker Container (on Port 80)**

bash
Copy
Edit
docker run -d -p 80:5000 flask-gif-app

**Access the App**

Local machine: http://localhost

On a cloud instance (EC2, etc.): http://<your-public-ip>

**Notes**

The app randomly selects a GIF URL from a predefined list.

Refreshing the page shows a new GIF.

Easy to extend with Giphy API for live GIFs.
