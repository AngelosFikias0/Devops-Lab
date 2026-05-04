# Docker Lab

A structured hands-on Docker engineering lab.

Not a collection of examples — a progressive learning system that moves from Docker fundamentals → multi-service architectures → production-like container systems.

---

## Purpose

Build deep practical competence in:

- Container lifecycle management
- Image creation and optimization
- Container networking
- Persistent storage and volumes
- Multi-service system design with Docker Compose
- Security fundamentals in containerized environments
- Performance constraints and resource control

Aligned with real-world DevOps and Platform Engineering workflows.

---

## Structure

Each folder is a conceptual layer. Work through them in order.

```
Docker-Lab/
├── 00-basics/              # Container lifecycle, core CLI, image fundamentals
│   ├── docker-run/
│   └── images-build/
├── 01-images/              # Image creation, layering, optimization
│   └── nginx-example/
├── 02-networks/            # Bridge, host, DNS, container communication
│   ├── bridge-network/
│   └── dns-resolution/
├── 03-volumes/             # Persistence, bind mounts, state management
│   └── persistence-demo/
├── 04-compose/             # Multi-container orchestration
│   ├── simple-stack/
│   └── multi-service-app/
├── 05-multi-service-systems/  # End-to-end: API + DB + proxy
│   └── api-db-nginx/
├── 06-security/            # User permissions, secrets, isolation
│   ├── user-permissions/
│   └── secrets-basics/
└── 07-performance/         # Resource limits, stress testing
    ├── resource-limits/
    └── cpu-memory-stress/
```

---

## Lab Structure

Every module follows the same pattern:

```
module/
├── README.md       # concept, objective, architecture, expected output
├── Dockerfile      # or docker-compose.yml
├── src/            # application code if needed
└── notes.md        # observations, failure cases, what you learned
```

Each README includes:
1. Concept definition
2. Minimal working example
3. Extended real-world scenario
4. Failure case or experiment
5. Key takeaways

No copy-paste tutorials. Everything is built and broken deliberately.

---

## How to Run a Lab

```bash
cd <module>

# Image-based
docker build -t lab-name .
docker run --rm lab-name

# Compose-based
docker compose up
docker compose down -v
```

---

## Progression Path

```
00 → 01 → 02 → 03 → 04 → 05 → 06 → 07
```

Do not skip modules. Each layer builds on the previous.

---

## Goals

This repository is maintained as part of a DevOps and Platform Engineering development path targeting:

- Cloud-native infrastructure
- Distributed systems design
- Kubernetes readiness
- Production-grade operational thinking

---

## License

Apache License
