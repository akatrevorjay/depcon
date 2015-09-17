# Depcon (*Container Deployment*)

[![Build Status](https://travis-ci.org/gondor/depcon.svg)](https://travis-ci.org/gondor/depcon) [![Go Documentation](http://img.shields.io/badge/go-documentation-blue.svg?style=flat-square)](http://godoc.org/github.com/gondor/depcon)  [![Join the chat at https://gitter.im/gondor/depcon](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/gondor/depcon?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) 

An advanced deployment tool for docker containers against Mesos/Marathon, Kubernetes and Amazon ECS

## Overview

Depcon makes managing clusters that run docker containers a breeze.  It offers the ability to define environments such as test, pre-prod, production against Marathon (initial release), Kubernetes and Amazon ECS.  

**Some key features of Depcon are:**
- Variable substistution in deployment descriptors
- Output results in Column, YAML and JSON formats for easy integration with automation
- Accepts deployment descriptors in either JSON or YAML format
- Full Mesos/Marathon support
  - Application, Group & Task management
  - Partial application updates: CPU, Memory & Scaling
  - Quick application rollback
  - Leader election, Server info and elapsed response
- Future releases will offer a proposed Open Deployment Descriptor format which will allow Depcon to deploy a common descriptor against Marathon, Kubernetes, ECS and Docker Swarm.
- Ability to wait until a new or updated container deployment is healthy

