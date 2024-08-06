# Welcome to SheerIoT

The purpose of this GitHub organization is to _SHARE_ IoT Know-How (KH) and How-To (HT).

Sheer means a lot of things. Look it up.

## Building an IoT Host (VM) on Azure or AWS

Start with a VM

- [Cloud VM](https://github.com/sheeriot/cloudvm) - a public repository that can be used to create environments and VMs on AWS and Azure.

1. Build Storage for Terraform State (aka tfstate) retention
1. Build Azure Network or AWS VPC
1. Build VM
1. Setup .ssh/config and connect

## Add Nginx for Web Hosting

Using this Repo:

- https://github.com/sheeriot/WebHostNginx

Currently needs Certbot managed manually.

## Surveyor - Now Public

The RF Field Surveyor (aka Surveyor) is a Django (python) web application that can be used to query an InfluxDB and provide LoRaWAN peformance data and visuals.

* [RF Field Surveyor - Public repo][(https://github.com/sheeriot/surveyor)

Here, a visual:

![RF Field Surveyor - Software Topology](https://github.com/sheeriot/surveyor/blob/trunk/README/surveyor/docs/diagrams/structurizr-1-RFFieldSurveyor.png)

# Archive....

This is where it began but these repos are now obsolete

Two repositories are now public:

* iotdash

    * use this terraform to create a new storage account (for terraform state), network, and virtual machine (linux) on Azure

* dashstack

    * forked and pruned from MCCI *docker-iot-dashboard*
    * creates an open-source docker-compose stack

        * nginx - a web server
        * mosquitto - an MQTT broker
        * node-red - flow-based programming (low-code) for IoT triggers and actions
        * influxdb - time-series data storage
