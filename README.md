### What is going on ?

- travis is watching github repo
- when main branch updates
  - travis runs the tests (client only for now)
  - if they pass:
    - travis uses docker to build 4 images
    - logs into my docker acct
    - and pushes the images to docker hub
  - aws.json file has Container Definitions (think: docker-compose file)

#### Notes

- ECS works with task definitions (instructions how to run a single container)
- one must be essential
- to connect, must add links to name (only has to be specified on one end)
- did travis stop working?
