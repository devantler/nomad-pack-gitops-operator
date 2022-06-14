# nomad-pack-gitops-operator

## Steps to MVP

- [ ] Create C# Project
- [ ] Listen and react to multiple webhook events / Run daily
- [ ] Run nomad-pack registry for all specified registries
- [ ] Check which nomad-packs have been updated based on registry version number vs currently deployed service number.
- [ ] Run nomad-pack run for all updated services. 

## Requirements for the Application

Secured webhook address + List of registries

Incoming webhook events should allow for dynamic setup of new deployment sources. E.g. a webhook from a private repository with nomad-packs, can be used to auto deploy those services to a cluster.

A list of registries should be supported as env variable to deploy from those registries daily.

Inclusive or exclusive filters on what to deploy should be added.
