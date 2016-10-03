# Rust and Containers launcher pattern

In this repository we share an example of "Rust and Containers launcher pattern" for the workshop [5 containers patterns for 5 languages](https://l0rd.github.io/talks/containers-and-languages/index_en.html).

```bash
# The following steps are commented out because 
# not necessary to run the example
# git clone https://github.com/containerslanguages/rust

# Build the rust app and package it withing a Docker image
# docker build -t containerslanguages/rust .

# Build the launcher image
# docker build -t containerslanguages/rust-launcher -f Dockerfile.launcher .

# Run the launcher
docker run --rm -v /var/run/docker.sock:/var/run/docker.sock 
           containerslanguages/rust-launcher start
```
