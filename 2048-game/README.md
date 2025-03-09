# 2048 Game

A lightweight containerized 2048 game, served with Nginx and deployable via Docker or Kubernetes.

Based on the original [Gabriele Cirulli's 2048](https://github.com/gabrielecirulli/2048), it requires no manual setup—just pull and run.

## 🌍 Running the Game

### Docker

```bash
docker pull zhernrong92/2048-game
docker run -d -p 8080:80 zhernrong92/2048-game
```
- Open http://localhost:8080 to play 🎮

### Kubernetes

```bash
kubectl apply -f k8s/deployment.yaml -f k8s/service.yaml
kubectl get svc  # Get external IP
```

- Access via the external IP or LoadBalancer URL.

## 📜 License
This repository contains code from the **2048 Game**, originally created by **Gabriele Cirulli**. The game itself is open-source under the **MIT License**.

