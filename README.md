# BBC-Bouncer
App that watches an ergo wallet and sends away unwanted token automatically.
## Setup
1. Clone the repository and enter the directory:

```
git clone https://github.com/rustinmyeye/BBC-Bouncer
```

```
cd BBC-Bouncer
```
   
2. Ensure Docker is installed on your system then, build the image with:
   

```
docker build -t BBC-Bouncer .
``` 

6. Then to start the container:

```
docker run -p 5000:5000 -d --name BBC-Bouncer BBC-Bouncer
```
