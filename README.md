# DeepFlow Agent

Zero-instrumentation observability agent using eBPF.
Captures HTTP, gRPC, SQL, NoSQL, MQ, DNS and more without code changes.

Reference: https://deepflow.io/docs/ce-install/legacy-host/

## Prerequisites

- DeepFlow Server running (docker-compose or K8s)
- Agent group already created on server (with config applied)

## Config

Edit `config/agent-config.yaml`:

- `controller-ips`: DeepFlow server IP
- `vtap-group-id-request`: agent group ID (from server)

## Run

```bash
docker compose up -d
```