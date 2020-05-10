# REST API and Docker


## Description
This is a simple Application using Flask. The FLASK app was uploaded in a Docker container. The REST API fetches departments, positions in those departments, names of the people having that position and salary of that one person when searched for.


# Running without Docker
In the command prompt:
## 1. Navigate to your cloned repository:
```
cd <your-address-here>
```
## 2. Install the required python libraries:
```
pip install -r requirements.txt
```
## 3. Run the application using:
```
python app.py
```

# Running with Docker Installed

## 1. Install Docker Desktop (for Mac / Windows)(Note: Only works for Windows 10 Pro / Enterprise)
## 2. Now you need to pull the image uploaded on the [Docker repository](https://hub.docker.com/r/sidduj/assignment-5), so for this:
## In the command prompt:
```
docker pull sidduj/assignment-5:latest
```
## 3. Then run the image you pulled using:
```
docker run sidduj/assignment-5
```
# Navigating the application
The highest view can be seen using the below link:
http://localhost:5000/departments

The detailed options under department can be seen using the below link:
http://localhost:5000/dept/law

Looking for an exact opsition can be done using the below link:
http://localhost:5000/dept/law/law%20clerk
## Note: Here '%20' denotes a space in between words

Finally, seeing a single person's entry/tuple from the database can be done using the below link:
http://localhost:5000/dept/law/law%20clerk/lim,%20%20teresa
