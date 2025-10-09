# Docker-Introduction
| Step       | Purpose                                          | Builds on                             |
| ---------- | ------------------------------------------------ | ------------------------------------- |
| **Task 1** | Create and run a static web app in Docker        | Base app running                      |
| **Task 2** | Add Keycloak with Docker Compose and link to app | App now has login system via Keycloak |



## TASK 1

Objective:

- Deploy a lightweight static web application inside a Docker container to understand image creation, container management, and application isolation.

1. Installed Docker and verified it works.

2. Cloned the GitHub repo (getting-started).

3. Created your own small app folder (my-app) with index.html and a Dockerfile.

4. Built your Docker image (suzy-docker-app).

5. Ran it inside a container (suzy-running-app) and confirmed it in your browser (http://localhost:8080).
   ![WhatsApp Image 2025-10-09 at 17 17 05_79cddac4](https://github.com/user-attachments/assets/ec205a21-1529-464f-bdfb-5c1bf2f036a3)

Concepts Learned:

- 🧱 Docker Image: A blueprint containing app code, dependencies, and runtime environment.

- 📦 Container: A running instance of the image — isolated yet lightweight.

- 🛠️ Dockerfile: Defines build instructions (base image, copy files, expose ports).

- 🌍 Port Mapping: Allows external access to a containerized app.
   
## TASK 2 
Objective 
- Install and configure a local Keycloak instance (Identity and Access Management system) using Docker Compose.

1. Create a docker-compose.yml defining both Keycloak and PostgreSQL services.

2. Configure environment variables (database name, username, passwords, admin credentials).

3. Run both services together using a single command:

- docker compose up -d


4. Access the Keycloak Admin Console at http://localhost:8080 to manage users, roles, and authentication.



| Phase | Focus                                        | Key Tool                  | Outcome                                         |
| ----- | -------------------------------------------- | ------------------------- | ----------------------------------------------- |
| **1** | Containerization of a web app                | Docker                    | Running a static app in an isolated environment |
| **2** | Multi-service orchestration & authentication | Docker Compose + Keycloak | Deploying a secure, scalable IAM system locally |

<img width="975" height="528" alt="image" src="https://github.com/user-attachments/assets/51c260ad-4461-4b6b-90ba-66b6b9ff1ada" />


A realm: myrealm

A client: my-app

A user: suzy

A role: user

