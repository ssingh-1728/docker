# Multi Stage Docker Build

Shared Dockerfile without-multi-stage results in 1GB image after build whereas Dockerfile with multi-stage i.e. distroless is just 152MB image after build.

# Distroless Advantages
1. Provide Security because only the minimal required package are present.
2. Small image size
