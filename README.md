# RisuAI-Docker
Dockerize https://github.com/kwaroran/RisuAI

### How to Use
- Start
  ```
  git clone https://github.com/thirdscam/RisuAI-Docker.git
  cd RisuAI-Docker
  docker compose up -d --build
  ```
- Upgrade
  ```
  docker-compose build --no-cache
  docker compose up -d
  ```