# HomeAssistant

## Commands

### Start container
  docker run -d --network=host --name homeassistant -v /etc/homeassistant:/config homeassistant/home-assistant

### Update to latest version
  docker stop home-assistant

  docker rm home-assistant

  docker pull homeassistant/home-assistant

  Start container

### MQTT
  sudo docker run -itd --name=mqtt --restart=always --net=host -v /storage/mosquitto/config:/mqtt/config:ro -v /storage/mosquitto/data:/mqtt/data -v /storage/mosquitto/log:/mqtt/log toke/mosquitto
