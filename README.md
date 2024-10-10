# INFO8985_monolith
otel for a python monolithic app

```bash
pip install -r requirements.txt
ansible-playbook playbook.yml
```

This is based on [the open telemetry docs](https://opentelemetry.io/docs/languages/python/getting-started/)

run `docker-compose up`. In another terminal window run:

```bash
export OTEL_PYTHON_LOGGING_AUTO_INSTRUMENTATION_ENABLED=true
opentelemetry-instrument --logs_exporter otlp flask run -p 8080
```


