---
title: Regions
layout: docs
sitemap: false
nav: firecracker
---

The Fly.io platform runs applications physically close to users: in datacenters around the world, on servers we run ourselves. We currently have servers in 21 regions:

## _Fly.io Regions_ ##



|Region ID| Region Location | Gateway |
|---------|-----------------|---------|
ams|Amsterdam, Netherlands      	| ✓
cdg|Paris, France               	| ✓
dfw|Dallas, Texas (US)          	| ✓
ewr|Secaucus, NJ (US)
fra|Frankfurt, Germany          	| ✓
gru|São Paulo
hkg|Hong Kong, Hong Kong        	| ✓
iad|Ashburn, Virginia (US)
lax|Los Angeles, California (US)	| ✓
lhr|London, United Kingdom      	| ✓
maa|Chennai (Madras), India     	| ✓
mad|Madrid, Spain
mia|Miami, Florida (US)
nrt|Tokyo, Japan                	| ✓
ord|Chicago, Illinois (US)      	| ✓
scl|Santiago, Chile             	| ✓
sea|Seattle, Washington (US)    	| ✓
sin|Singapore                   	| ✓
sjc|Sunnyvale, California (US)  	| ✓
syd|Sydney, Australia           	| ✓
yyz|Toronto, Canada             	| ✓

## _Discovering your Application's Region_

You can see the list of Fly.io regions any time with [`fly platform regions`](https://fly.io/docs/flyctl/platform-regions).

You can see which regions your app is running in with [`fly status`](https://fly.io/docs/flyctl/status/).

View and manage your app's region pool with [`fly regions`](/docs/flyctl/regions/). See [Scaling and Autoscaling](/docs/reference/scaling/) for more about regions and scaling.

Fly.io [storage volumes](/docs/reference/volumes/) are tied to the region they're created in. 

When an application instance is started, the three-letter name for the region it's running in is stored in the VM's `FLY_REGION`  environment variable. This, along with other [Runtime Enviroment](/docs/reference/runtime-environment/) information, is visible to your app running on that instance.