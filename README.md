# SDS
Software-Defined Systems

## exercise 1
### Hints
1. Check the toyota-data-feeder repository
2. Create a Dockerfile that executes feeder.py on container startup
   Only include files that are actually needed for the application to run
   For example, be sure to not include /assets folder in your image
3. Build the image and push it to the registry
   You can use either DockerHub or CSC Rahti registry, but we recommend the latter.
   If you are using CSC Rahti registry, be sure to assign assistants to your project and to change image pull policy to Anonymous. Check exercise 1 slides for more.
4. Tag the image with 1.0 tag
   Run the image with correct MQTT_URL, MQTT_PORT  and CLIENT_ID values
   Don't hardcode these values!
5. Use mosquitto_sub to confirm you are receiving messages from your Docker container
   Use flags --verbose --insecure and --cafile ca.crt. Get ca.crt and other certificates from exercises page.
6. Execute a command which lists working directory's files of the running container  (that directory where you copied application files in step 2)


### Deliverables
1. Dockerfile, and other files if needed.
2. Small text report with the commands and outputs of each step (except step 2)
   Include your name and CSC Rahti account name in this text file
   Please, don't copy-paste the whole output when data is being sent/received, just a small snippet. (Steps 4,5)
    
### My Text Report
1. open [toyota-data-feeder](https://github.com/smaddis/toyota-data-feeder) to download the zip and unzip it ![ToyotFolder](materials of sds exe1/TF.png)
