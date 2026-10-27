# Raspberry Pi home server

A personal server I set up on a Raspberry Pi to host my projects, collect sensor data and monitor everything from one dashboard.

I use it alongside my embedded projects, including [Plant Tracker](https://github.com/idk-sheesh/plant-tracker). It has also been a way to learn Linux administration beyond getting a service to start once.

## What it does

- Runs personal services with Docker Compose and persistent NVMe storage.
- Shows system metrics, service health and backup results in a custom web dashboard.
- Collects readings from ESP32 sensor nodes.
- Automates encrypted backups, with integrity checks and test restores.
- Provides DNS filtering for local devices.

## My work

I set up the Linux host and storage, deployed the services and built the monitoring hub with Python, HTML, CSS and JavaScript. I also worked on backup automation and the less visible parts: file permissions, restart behaviour, offline devices and recovery checks.

One useful lesson was that a successful backup job does not prove the data can be restored. The dashboard distinguishes backup results from restore checks, and flags failures or outdated readings instead of leaving an old success on screen.

## Stack

Raspberry Pi, Debian, Python, HTML/CSS/JavaScript, Docker Compose, SQLite, Restic and AdGuard Home.

## Status

Deployed and used for personal projects. I continue to improve the monitoring and maintenance tools as new devices and services are added.

This repository is a public project overview. Deployment files and operational documentation are kept private.
