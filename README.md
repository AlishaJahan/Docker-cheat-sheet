# Docker-cheat-sheet
| Command            | Description                   |
| ------------------ | ----------------------------- |
| `docker --version` | Show Docker version           |
| `docker info`      | Show system-wide Docker info  |
| `docker help`      | Get help with Docker commands |

Working with Images
| Command                          | Description                 |
| -------------------------------- | --------------------------- |
| `docker pull <image>`            | Pull image from Docker Hub  |
| `docker images`                  | List local images           |
| `docker rmi <image_id>`          | Remove image                |
| `docker build -t <name>:<tag> .` | Build image from Dockerfile |

Working with Containers
| Command                               | Description                 |
| ------------------------------------- | --------------------------- |
| `docker run <image>`                  | Run container from image    |
| `docker run -it <image>`              | Run with interactive shell  |
| `docker run -d <image>`               | Run in detached mode        |
| `docker run -p 8080:80 <image>`       | Map ports (host\:container) |
| `docker ps`                           | List running containers     |
| `docker ps -a`                        | List all containers         |
| `docker stop <container_id>`          | Stop container              |
| `docker start <container_id>`         | Start container             |
| `docker restart <container_id>`       | Restart container           |
| `docker rm <container_id>`            | Remove container            |
| `docker exec -it <container_id> bash` | Open shell inside container |
| `docker logs <container_id>`          | View container logs         |

Docker-compose commands
| Command                | Description                |
| ---------------------- | -------------------------- |
| `docker-compose up`    | Start services             |
| `docker-compose up -d` | Start in detached mode     |
| `docker-compose down`  | Stop and remove containers |
| `docker-compose build` | Build images               |
| `docker-compose ps`    | List services              |

Volumes & Bind Mounts
| Command                                | Description            |
| -------------------------------------- | ---------------------- |
| `docker volume create <name>`          | Create volume          |
| `docker volume ls`                     | List volumes           |
| `docker run -v <volume>:/data <image>` | Attach volume          |
| `docker run -v $(pwd):/app <image>`    | Bind mount current dir |



