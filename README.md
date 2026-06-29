# Full Stack Fundamentals, v3 — Notes & Projects

My notes and hands-on projects from the [**Full Stack Fundamentals, v3**](https://frontendmasters.com/courses/fullstack-v3/) course by [Jem Young](https://www.linkedin.com/in/jemyoung/) (working at **Netflix** at the time of recording) on Frontend Masters.

It covers the full breadth of what it means to run software in production — from the command line and operating system fundamentals, through networking, server setup, security, CI/CD, real-time communication, databases, and finally containers and orchestration.

- 📚 **Course:** https://frontendmasters.com/courses/fullstack-v3/
- 📝 **Official notes:** available as a downloadable PDF
- 👤 **My learning profile:** https://frontendmasters.com/u/okshanaby/

---

## What's inside

Each numbered folder is one section of the course. The `.md` files are my written notes; the subfolders are the working projects built along the way.

| Section | Topic | Highlights |
| --- | --- | --- |
| **1. Command Line** | Shell basics | Shell fundamentals, navigating the terminal |
| **2. Servers** | Running a server | Simple Node.js server, hands-on exercise |
| **3. Operating System** | OS, security & SSH | OS overview, hashing, SSH keys, keychain & agent |
| **4. The Internet** | Networking & DNS | How the internet works, network tools, DNS, buying a domain, server & user setup, file permissions |
| **5. Application Setup** | NGINX, Node.js & PM2 | Setting up NGINX, deploying a Node.js app, proxy pass, virtual servers, PM2 process manager |
| **6. GIT** | Version control | Git fundamentals and version control workflows |
| **7. Security** | Hardening a server | Ports, firewall with ufw, file permissions, unattended upgrades |
| **8. CI & Deployment** | Automation & ops | CI/CD pipelines, cron jobs, logging/streams/redirection, find & grep, NGINX gzip & redirects, subdomains |
| **9. Realtime & Databases** | WebSockets, SQLite & HTTPS | WebSocket protocol, Express integration, SQLite, HTTP/HTTPS overview, Certbot TLS, HTTP/2 |
| **10. Containers** | Docker & orchestration | Containers overview, running Docker containers, orchestration, load balancers |

### Project folders

- **`2. Servers/exercise`** — a simple Node.js server built during the servers section.
- **`frontendmasterslearningxyz`** — the running project used throughout the course: a Node/Express app with WebSocket support (`index-ws.js`), a static front end (`index.html`), and a CI simulator script (`ci-simulator.sh`).

---

## Key concepts covered

- **Command line & shell** — navigating the filesystem, writing shell scripts, and feeling at home in the terminal.
- **Servers** — what a server is and how to write and run a minimal Node.js HTTP server.
- **Operating system** — how an OS manages processes and resources, security fundamentals, hashing passwords, and SSH key-based authentication.
- **Networking & DNS** — the full journey of an HTTP request, DNS resolution, buying and configuring a domain, and provisioning a cloud server.
- **Application setup** — installing NGINX as a reverse proxy, deploying a Node.js application, configuring virtual servers, and keeping the app alive with PM2.
- **Security** — closing unnecessary ports, configuring a firewall with `ufw`, tightening file permissions, and enabling automatic security upgrades.
- **CI & Deployment** — building a continuous integration workflow with cron, understanding log streams and redirection, searching with `find`/`grep`, enabling gzip compression and NGINX redirects, and setting up subdomains.
- **Realtime & databases** — the WebSocket protocol, adding real-time communication to an Express app, persisting data with SQLite, and upgrading to HTTPS/HTTP 2 with Certbot.
- **Containers** — what containers are, running and managing Docker containers, and orchestrating multi-container applications behind a load balancer.

---

## Getting started

You'll need [Node.js](https://nodejs.org/), [NGINX](https://nginx.org/), and [Docker](https://docs.docker.com/get-docker/) installed depending on which section you're following.

```sh
# Clone
git clone <this-repo-url>
cd fullstack-fundamentals-v3

# Run the course project locally
cd frontendmasterslearningxyz
npm install
node app.js
```

> The notes are best read top to bottom, section by section — they build on each other.

---

## Acknowledgements

All credit for the course material goes to **Jem Young** and **Frontend Masters**. This repository is my personal study log while taking the course.
