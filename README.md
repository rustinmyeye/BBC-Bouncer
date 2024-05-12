# BBC-Bouncer
Welcome to BBC-Bouncer! This application automatically monitors a wallet for specific token IDs and bounces (sends to burn address) any tokens found. Checks for the blacklisted token IDs happen every 5 minutes.
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

3. Then to start the container:

```
docker run -p 5000:5000 -d --name BBC-Bouncer BBC-Bouncer
```
4. Navigate to the web ui at `http://localhost:5000`
5. Enter your mnemonic in the provided field below and click "Set Mnemonic".
6. Enter the Token ID's you want to bounce (separated by commas) in the field below and click "Set Token IDs".
