# Installation

### Docker Compose

For Docker usage, please install docker and docker-compose and fill up the \*.env file inside the conversational-hub-docker folder.

```
conversational-hub-docker.yml
---
version: '3'
services:
  frontend:
    image: registry.connect.redhat.com/captivateioltd/frontend
    container_name: frontend
    ports:
      - '80:8080'
    env_file:
      - frontend.env
    depends_on:
      - chatbot
    networks:
      - app-network

  chatbot:
    image: registry.connect.redhat.com/captivateioltd/chatbot
    container_name: chatbot
    ports:
      - '8084:8080'
    env_file:
      - chatbot.env
    depends_on:
      - mongodb
      - redis
      - rabbit
    networks:
      - app-network

  channel-gateway:
    image: registry.connect.redhat.com/captivateioltd/channel
    container_name: channel-gateway
    ports:
      - '8085:8080'
    env_file:
      - channel-gateway.env
    depends_on:
      - chatbot
      - mongodb
      - redis
      - rabbit
    networks:
      - app-network

  livechat-gateway:
    image: registry.connect.redhat.com/captivateioltd/livechat
    container_name: livechat-gateway
    ports:
      - '8086:8080'
    env_file:
      - livechat-gateway.env
    depends_on:
      - chatbot
      - mongodb
      - redis
      - rabbit
    networks:
      - app-network

  mongodb:
    image: registry.access.redhat.com/rhscl/mongodb-36-rhel7
    env_file:
      - mongodb.env
    networks:
      - app-network

  redis:
    image: registry.redhat.io/rhel8/redis-5
    env_file:
      - redis.env
    networks:
      - app-network

  rabbit:
    image: registry.connect.redhat.com/captivateioltd/rabbitmq
    env_file:
      - rabbit.env
    networks:
      - app-network

networks:
  app-network:
    driver: bridge
```

```
docker-compose -f conversational-hub-docker.yml up
```

### Helm Charts (k8s/Openshift)

For Kubernetes and Minikubes installation, we recommend you to download helm from this [link](https://github.com/helm/helm/releases) and install it to your machine. Configure the helm to your kubernetes master, modify the `*-env-configmap.yaml` inside `conversational-hub-helm/templates` . and run the command inside the ch-helm folder

```
helm install ./conversational-hub-helm --generate-name
```

You can also generate your own helm charts by converting the docker-compose.yml using [kompose](https://kompose.io/)

Reminder: If you’re using the latest version of Kubernetes (>1.16) please modify apiVersion of `conversational-hub-helm/templates/app-network-networkpolicy.yaml` to `networking.k8s.io/v1`

Kubernetes < 1.16

```
apiVersion: extensions/v1beta1
```

Kubernetes > 1.16

```
apiVersion: networking.k8s.io/v1
```

### OpenShift Operator

&#x20;For Openshift Container Platform, login to your `Redhat Openshift Container Platform`, go to `Operator Hub` and search for `Conversational Hub` to find the instructions.

