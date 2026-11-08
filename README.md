# platform-observability

This repository currently documents the intended observability platform; it
does not contain telemetry collectors, service instrumentation, dashboards,
alert rules, or SLO definitions. Treat those capabilities as planned here,
not as implemented by this repository.

The related `platform-infrastructure` repository documents Terraform-managed
CloudWatch dashboards and alarms plus the EKS CloudWatch Observability add-on
for cluster and container logs/metrics. It also notes that applications expose
Actuator health and Prometheus metrics, but no Prometheus scraper,
long-term application-metrics store, or OpenTelemetry trace collector/backend
is provisioned there. Verify the owning infrastructure configuration and
deployment before relying on any signal for alerting or service objectives.

Cross-repository architecture decisions are tracked in the canonical [Product
Platform ADR index](https://github.com/Jahrough/ai-native-engineering/blob/main/docs/architecture/adr/README.md).
Those records are proposals unless explicit approval is recorded; they do not
imply implementation or deployment.
