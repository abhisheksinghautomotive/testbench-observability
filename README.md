# Observability for ECU Test Pipelines 🚦

A production-grade observability platform for monitoring, debugging, and optimizing the full HIL/SIL ECU test lifecycle — from reservation → provisioning → execution → teardown.

---

## 📌 What This Project Provides

* Unified **metrics, logs, and traces** across benches, orchestrator, workers, and CI.
* **Dashboards** for ops, developers, and business teams.
* **Alerting** with runbooks for P1/P2 issues.
* **Retention, cost control, and RBAC** for secure and scalable operations.
* **Correlation IDs** everywhere for end-to-end debugging.

---

## 🧱 Core Components

* **Metrics:** Prometheus (with optional long-term storage).
* **Logs:** Loki or CloudWatch Logs with structured JSON.
* **Tracing:** OpenTelemetry → Jaeger or AWS X-Ray.
* **Dashboards:** Grafana (Ops, Execution, Developer, Cost, SLO).
* **Alerting:** Alertmanager → Slack/SNS/PagerDuty.
* **Collectors & Exporters:** OpenTelemetry Collector and service-level instrumentation helpers.

---

## 🔧 What Gets Instrumented

* Orchestrator
* Bench hosts
* Workers and runners
* CI pipelines
* Test executions and results

All telemetry includes: `correlation_id`, `environment`, `team`, `bench_id`.

---

## 📁 Repository Structure

```
observability/
├─ dashboards/
├─ alerting/
├─ collectors/
├─ exporters/
├─ helm/
├─ tests/
├─ docs/
│  └─ RUNBOOK.md
└─ .github/workflows/
```

---

## 🚨 Key Features

* End-to-end test tracing
* Bench utilization and queue latency metrics
* Error heatmaps and flaky test analysis
* Cost and ingestion monitoring
* Runbooks for every P1/P2 alert
* 30-day hot retention + 1-year archival

---

## 🔄 Integrations

* Infra outputs from Project A
* Instrumentation libraries from Project B
* CI for validating dashboards, rules, and synthetic telemetry tests

---

## 🎯 Goals

Reliable visibility into system health, faster RCA via traces, predictable alerting, and long-term telemetry retention with cost efficiency.

---

## License

This project is licensed under the MIT License. See the LICENSE file for details.

---
