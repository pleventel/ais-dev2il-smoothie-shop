# DEV2IL: Observability

## Getting Started

- [Getting Started](./01_GETTING_STARTED.md)

## Logging

- [Operating the Smoothie Shop](./02_OPERATING_SMOOTHIE_SHOP.md)
- [Providing More Insights Through Log Outputs](./03_LOGGING_BASICS.md)
- [Collecting Logs in a Central Place](./04_CENTRAL_LOGGING.md)

## Metrics

- [Collecting Metrics with Prometheus](./05_METRICS.md)

## Tracing

- [Distributed Tracing with Jaeger](./06_TRACING.md)

## Troubleshooting 

### `docker-compose` Networking / Orphaned Container Troubles

If you experience any problems with `docker-compose` and networks not being found, e.g. 
```
Error response from daemon: failed to set up container networking: network 63e3d803b202b6c38f0e3aebbb5890a057757a9b04939500ee339e0153659e59 not found
```
then try to restart your docker-compose managed services using 
`docker-compose down --remove-orphans && docker-compose up -d` 

## Further Readings

Logging
- https://docs.python.org/3/howto/logging.html
- https://docs.python.org/3/library/logging.html
- https://grafana.com/docs/loki/latest/query

Metrics
- https://prometheus.io/docs/concepts/metric_types/
- https://prometheus.io/docs/prometheus/latest/querying/basics/
- https://prometheus.io/docs/alerting/latest/overview/

Tracing
- https://opentelemetry.io/docs/concepts/
- https://opentelemetry.io/docs/concepts/instrumentation/zero-code/