# nomad-pack-gitops-operator

This is a WIP.

## Steps to MVP

- [ ] Create C# Project, Dockerfile and GitHub Action with Nightly and Releases pipeline. 
- [ ] Listen and react to multiple webhook events for dynamic configuration of deployment sources / Run at timed intervals for manual deployment sources.
- [ ] Run nomad-pack registry for all specified registries
- [ ] Check which nomad-packs have been updated based on registry version number vs currently deployed service number.
- [ ] Run nomad-pack run for all updated services.

## Requirements for the Application

Secured webhook address + List of registries

Incoming webhook events should allow for dynamic setup of new deployment sources. E.g. a webhook from a private repository with nomad-packs, can be used to auto deploy those services to a cluster.

A list of registries should be supported as env variable to deploy from those registries at timed intervals.

Inclusive or exclusive filters on what to deploy should be added.
