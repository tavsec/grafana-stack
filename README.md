# grafana-stack

## Requirements

- Access to AWS S3, and configured credentials
- Buckets created on S3:
  - tempo
  - loki_data
  - loki_ruler



## Setup

```bash
docker-compose up -d
```

Update values in .env file.

## Endpoints

Zipkin OTEL endpoint:
`http://localhost:9411`

## Open ports
| Port  | Description       |
|-------|-------------------|
| 14268 | jaeger            |
| 3200  | tempo             |
| 9411  | zipkin            |
| 9001  | minio             |
| 9090  | prometheus        |
| 3000  | grafana dashboard |
| 3101  | loki              |
| 7946  | loki              |
| 9095  | loki              |
| 3100  | loki gateway      |
