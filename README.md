# HomeAssistant

## Commands

### Start container
  docker run -d --network=host --name homeassistant -v /etc/homeassistant:/config homeassistant/home-assistant

### Update to latest version
  docker stop home-assistant

  docker rm home-assistant

  docker pull homeassistant/home-assistant

  Start container
