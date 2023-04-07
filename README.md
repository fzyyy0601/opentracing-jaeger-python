# jaeger + OpenTracing + python

A simple project using Python to implement OpenTracing with Jaeger followed this tutorial(https://medium.com/velotio-perspectives/a-comprehensive-tutorial-to-implementing-opentracing-with-jaeger-a01752e1a8ce)

## Prerequisite
```bash
python3 -m pip install jaeger-client
python3 -m pip install opentracing_instrumentation
```

## Run Jaeger as backend in Docker image
```bash
docker run -d -p6831:6831/udp -p16686:16686 jaegertracing/all-in-one:latest
```

## Run the python program
```bash
python booking-mgr.py <movie-name>
```

## Accessing Jaeger dashboard
Open browser and go to http://127.0.0.1:16686/;