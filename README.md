# flowsuite

`flowsuite` is a Docker image containing several Bioconductor packages dedicated to the analysis
of flow cytometry data.

## Build image

```
docker build -t tercen/flowsuite:0.0.4 .
docker push tercen/flowsuite:0.0.4
```

## Inspect image

```
docker run -it --entrypoint=bash tercen/flowsuite:0.0.4
```
