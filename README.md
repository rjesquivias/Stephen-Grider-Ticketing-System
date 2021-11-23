# Steps to initialize a new microservice in js
1. Create a new directory
2. npm init -y
3. install dependencies (e.g. npm install typescript ts-node-dev express @types/express)
4. tsc --init (if working with typescript)
5. Set up a start script within package.json
    - "start": "nodemon index.js" if on js
    - "start": "ts-node-dev src/index.ts" if on ts

# Next steps to setup docker/kubernetes
1. Setup Dockerfile & .dockerignore
2. Ensure docker can successfully build and run the image
3. Setup k8s infra (basic deployment and clusterip)
4. Setup skaffold config to copy any code changes to code files to the correct container and rebuild infrastructure on k8s file changes
5. Test infra with 'skaffold dev'