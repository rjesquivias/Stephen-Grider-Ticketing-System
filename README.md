# Steps to initialize a new microservice in js
1. Create a new directory
2. npm init -y
3. install dependencies (e.g. npm install typescript ts-node-dev express @types/express)
4. tsc --init (if working with typescript)
5. Set up a start script within package.json
    - "start": "nodemon index.js" if on js
    - "start": "ts-node-dev src/index.ts" if on ts