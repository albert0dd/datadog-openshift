# datadog-openshift

For deploying opentelemetry integrated collector in openshift, get values and otel config from otel directory and:
helm install dd -f  agent_on_openshift_values.yaml --set datadog.otelCollector.enabled=true --set-file datadog.otelcollector.config=otel_collector_config.yaml -n datadog datadog/datadog
