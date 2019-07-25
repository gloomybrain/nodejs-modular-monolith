# Nodejs Modular Monolith

## Docker
```bash
docker build -t <your username>/node-modular-monolith

docker run -p 3000:3000 -d <your username>/node-web-app
```

## Component
- domain module: modul yang berhubungan dengan bisnis proses
  - controller: melakukan request, response, validation
  - service: bisnis logic.
  - repository: satu2nya component yang secara langsung mengakses DB
  - plain function
  - plain object
- shared module
  - plain function
  - plain object
  - constant
- infastructure module
  - configs
  - database
  - logger
- router.js: list route
- server.js: bootstraping all module
- app.js: entry point

## TODO
- dockerize app
- add test suit