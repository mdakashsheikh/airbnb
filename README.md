# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...

## Install Ruby || Install gems || Precompile assets || Build your app image
```bash
docker build -t airbnb . 
```

## Get Your Rails Master Key
```bash
config/master.key
```

```bash
cat config/master.key
```

## Run the Container

```bash
docker run -d -p 80:80 \
-e RAILS_MASTER_KEY=your_master_key_here \
--name airbnb airbnb
```

## Replace:
your_master_key_here

## Run
```bash
docker compose up --build
```

## Summary
```bash
docker build -t airbnb .
```
```bash
docker run -d -p 80:80 -e RAILS_MASTER_KEY=... airbnb
```

