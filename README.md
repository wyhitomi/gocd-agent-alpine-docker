# GoCD Agent + docker

# Running

```
docker \
  run \
  -d \
  --rm \
  -v /var/run/docker.sock:/var/run/docker.sock \
  -e GO_SERVER_URL: "https://gocd-server:8154/go" \
  -e AGENT_AUTO_REGISTER_KEY: "your auto register key" \
  -e AGENT_AUTO_REGISTER_RESOURCES: "docker" \
  -e AGENT_AUTO_REGISTER_ENVIRONMENTS: "your environments" \
  -e AGENT_AUTO_REGISTER_HOSTNAME: "alpine-docker" \
  wyhitomi/gocd-agent-alpine-docker:v18.7.0
```
