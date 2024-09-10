# Sandbox to Production Guide

## Introduction
This sandbox is for development purposes.  While developing, we generally provide full access to sandbox and run with minimal resources.  However, in production there are many aspects that need to be taken care. This guide highlights some of the production related changes that need to be implemented while going produduction. 

## External API access
Only allowed APIs given external access.

## Protection of secrets

## Config server
* Tight controlled access
* Local mosip config repo with tight control

## Local docker registry
For local access of all docker images

## TPM 

## Reg client settings
* Max upload document size
* Max packets remaining to upload

## Console machine access
* User creation
* K8s access

## K8s master HA cluster

## Cluster roles and access
K8s cluster roles, policies and access

## Nginx between abis and activemq

## Rolling updates
[Rolling updates](rolling_updates.md)

## Kubernetes Pod config
* Replication
* CPU/Memory allocation
* [Reference config](../utils/production)

## Policies
* Review the expiry time of ABIS and other partner policies where data is shared.

## Firewalls 
* Between mz and dmz
* Between nginx and dmz

## Persistence

## Keycloak
* Review token timeouts and other expiries.

## Config properties
* Update batch job timing to suit the local time.  

## Reg proc stages
* Remove unused stages in reg proc (for example External Stage if not being used).

## Reprocessor
Reprocessor frequency

## Email/SMS gateway

## Activemq
* Memory settings
* High availability configuration

## On field operations/troublehshooting
* If activemq is restarted then ABIS service may need a restart to connect to the Q again.
* If idschema / ui schema is changed in the DB, then idrepo must be restarted. 


## BioSDK service setup 
